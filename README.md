# simple-modal-libraryA library of React components created using `create-react-app`.

## 1/ InstallationRun the following command:

`npm install simple-modal-library`


### 2/ Import the component from the library :

`import { Modal } from 'simple-modal-library'`
`import React from 'react'`
`import styles from "./style.module.css"`


### 3/ Place this state hook (concerning the opening/closing of the modal) at the start of the function that uses the Modal component :

`cconst [showModal, setShowModal] = useState(false)`

### 4/ In the return of the function, call the Modal component :

`{showModal && (<Modal className={styles["box-modal"]} message="Employee Created!" onClose={closeModal} /> )}`


### 5/ Example :

```js
import React, { useState } from 'react'
import { Modal } from '../components/Modal'

export default function Home() {
  const [isOpen, setIsOpen] = useState(false)
  const name = 'John Smith'

  return (
    <>
      <h1>Modal Test</h1>
      <button onClick={() => setIsOpen(true)}>Open Modal</button>
      {showModal && (
        <Modal className={styles["box-modal"]} message="Employee Created!" onClose={closeModal} />
      )}
    </>
  )
}
```


## Prerequisites

![npm](https://img.shields.io/badge/npm-9.1.3-%23000000?style=flat-square&logo=npm&logoColor=white)

![yarn](https://img.shields.io/badge/yarn-1.22.19-%232C8EBB?style=flat-square&logo=yarn&logoColor=white)

![Node.js](https://img.shields.io/badge/Node.js-16.14.0-43853D?style=flat-square&logo=node.js&logoColor=white)

## Dependencies

![GitHub package.json dependencies (dev)](https://img.shields.io/github/package-json/dependency-version/FABIEN-T/P14-modal-react/react?label=REACT&logo=react&logoColor=61DAFB&color=303540&style=flat-square)

![GitHub package.json dependencies (dev)](https://img.shields.io/github/package-json/dependency-version/FABIEN-T/P14-modal-react/react-dom?label=REACT-DOM&logo=react&logoColor=61DAFB&color=303540&style=flat-square)

![GitHub package.json dependencies (dev)](https://img.shields.io/github/package-json/dependency-version/FABIEN-T/P14-modal-react/styled-components?label=Styled-Components&logo=styled-components&logoColor=b758ad&color=b758ad&style=flat-square)

### DevDependencies

<!-- ![GitHub package.json devDependencies version (dev)](https://img.shields.io/github/package-json/devDependency-version/FABIEN-T/P14-modal-react/prop-types?label=Prop-types&color=303540&style=flat-square) -->

![Prop-types](https://img.shields.io/badge/Prettier-^2.8.2-blue?style=flat-square)

![Prettier](https://img.shields.io/badge/Prop--types-%5E15.8.1-blue)

![Vite](https://img.shields.io/badge/Vite-^4.3.5-blue?style=flat-square)