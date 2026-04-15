# 🚀 Essential Data Structures Guide

A clean and visual guide to fundamental data structures with **TypeScript examples**.

---

# 🔹 ARRAY

## 📘 Overview
👉 Stores data in **continuous memory (index-based)**

- Access: `O(1)`
- Insert: `O(n)`
- Size: Fixed

### 🖼️ Visualization

![Image](https://images.openai.com/static-rsc-4/TaRLkT1f2jEiHxqhcMSrGUfGlvpYI1jbE0RPamDe8BsuDce2G9qUKBa5ZvRxBBoargpr4jq_gzIMP-nswRfrmRJWWMK75lTwGcdl8htmemD2LXRQ6hpvKOxXzAJ3acFurXJNT7MqYgw-vxJ6C4wnKvwKkSMpt3hYGkPBSEBy3O4Jd6b9HJEh9Q9ZMKVak5rQ)
![Image](https://images.openai.com/static-rsc-4/e6rDD65S5UIcQzyodw52OnLJWcMMf3Kc7imcvVAjmUTL-uY5SlEfU0oAXw2Rdl5bT0Tb-Xmr40oCtpzURYDsMlxWvRI42ORLSPbZC5NQfs2MMEa7hn1ybNxIJZpLJUUSq9scCH1zXBIZM2DwXdgI9sl4OCTmdA5B5lDi6XAuzmqHpPXd0bnynozRWqJxaYXk)
![Image](https://images.openai.com/static-rsc-4/ybCMUKY8xHCT-Rc9rtfTTHdaO2w0wHpqcq0jm7enHe_nw0aIOQfSyLddcXvKG2WpyhBxuyF_Qb_S47KVjDt4qYbXRVVvBKjQ6mbMNt6_sSnaLCE7vFI9UlyvtbpkcCUq6LBkK7Um330ONF0WkVsJymPChWO4vM_qocDtipHpDLAi2NHXbDxreagL5ZHD2kOX)
![Image](https://images.openai.com/static-rsc-4/v2TvNKq8sx8EmYu5UXQt4w_HplC7a6WG3jRFwFp6AdbnzWjoJ6-B__k7ohiL3fjb6TwKvPMOKYaKR9Op81YmS03O5nMKlEzdFqKJGuBLpIRp9v7ZHAwSsTcMjqF4uEm6sZoX8Y7em2ZWrpRM21JzWR1EVJ2jqDpRb7wSutCnXifQ65rOsG7R5R7Gigd02g-C)
![Image](https://images.openai.com/static-rsc-4/N-7jg9gNFD9Ih_91L5qnV2aPNJEpfDmT9pVn8oJvo24hlmE_AVhFX9gYSv6HyizKO_EUO-kiIWLVbBWBajYf4RY43JAhpPzfRKXdRZuXqFzR_TSZKzF2yjj8Ewx6NQ6GDwU0Xj53l3jz9XoRt0s325ZPfbQ90qgGXhUf4LXyggzUvYXz54tnnLKM1m2whVDu)

### 💡 TypeScript Example
```ts
const arr: number[] = [10, 20, 30];

console.log("First element:", arr[0]);
console.log("Second element:", arr[1]);
````

---

# 🔹 LINKED LIST

## 📘 Overview

👉 Nodes connected using **pointers (links)**

* Dynamic size
* Access: `O(n)`

### 🖼️ Visualization

![Image](https://images.openai.com/static-rsc-4/FFb5yyqbY0pmw_8jJJtjCzsE7VMYsGZKNdPdGRDtkKjQpBnqg_aIQHJL7Zkp7_1f9CuS1yERPFumom-umdqMijsgRNVFKLL5iTCFsISPIWz48HYlCrQLuuvUjGLMKIPjW77ai1Ed_EnF6_rPFEbdsJHbSfRCZnF6BdHDjYQjYFDhRaOAGhp6HTfH588VkzE-)
![Image](https://images.openai.com/static-rsc-4/QakWb0GMOF8EZSDmAA6PZtc7xJpY_EujBhIPdq_y2crCW7DZFSVaJe9y3iX-2M2pCP8ybamdE1fD1EALPhgf4jtWrD7ZjIkOXKPPbVh1Nh3lAYrB1RXQCeuVUrNUqO6DKGXVUFtQjfuTbhCipX-7Drt45IQd6oiGlU028yR2WjH9X58Y0-zWxzfiu_n5V4KB)
![Image](https://images.openai.com/static-rsc-4/50Q8HBSIuBoWjjdhl6wZuWK3gKj45uFhqKscEAwrJrU_igKIYkhE9YkRglsefcog4u5k0Lib6tSlCb7ItMC7VZRXJDLCW0uLf2NUt_AZl6NMIfwDii2k-6CoxMKz0uEImOh5e8b52tNehREG9aVObt6WNWrgw_3hCvNQmSQYMa3Tx1WhhBvBQ7yp7w8OmUeY)

### 💡 TypeScript Example

```ts
class Node {
  data: number;
  next: Node | null;

  constructor(data: number) {
    this.data = data;
    this.next = null;
  }
}

const first = new Node(10);
const second = new Node(20);

first.next = second;

console.log(first.data);
```

---

# 🔹 STACK (LIFO)

## 📘 Overview

👉 Last In, First Out

### 🖼️ Visualization

![Image](https://images.openai.com/static-rsc-4/sCGRMVbsNW_S8GA9t7jEzOHs0kpvNca6sw19QswvLbnwglt7dRAUYJYPzNiMKOvi2voTA8IOuOzxZkLr4Nvjb3gVq0DePlHZL9KP-bOtZ5EY5WwM9NPk4t7cgjLJ79ew5JAqk71s3DN80EEeQET6vBUN5icI_3Baac8uu6V9Z7eBYftt3P-3Wvx3_qcKvqTS)

### 💡 TypeScript Example

```ts
const stack: number[] = [];

stack.push(10);
stack.push(20);

console.log(stack.pop());
```

---

# 🔹 QUEUE (FIFO)

## 📘 Overview

👉 First In, First Out

### 🖼️ Visualization

![Image](https://images.openai.com/static-rsc-4/gKe7KcryN06QY5O64wiB7s6xrWj3lk60P4THzYpRYohv6ssR3mSCOoNb_WKVSzk939sdtWki0oZXx9JfsrNuctbTaFNBLb430X6DE6kqHL9CJngvoi0AmT1Telpc-yjtei_MtQiBXT84yqxpjsD_gx2aOXx5hVh8CGw_PENhMV6EsUvgt2D7sfbcV6e_ohik)

### 💡 TypeScript Example

```ts
const queue: number[] = [];

queue.push(10);
queue.push(20);

console.log(queue.shift());
```

---

# 🔹 TREE

## 📘 Overview

👉 Hierarchical structure (Parent → Child)

### 🖼️ Visualization

![Image](https://images.openai.com/static-rsc-4/zDODzMZ0aiiyH31cbCl_fQGsv7E-Ag1Il6jrOYSWXbyKDMr_qGehWYFwJ4vu03FB4JIMJmUmjMAjPHufFs0P0KYcd4IkokXgsFWvMbv7_TtZQNQy8rIH61du31dAQLc3AvMqhXqOqzc_E8c_XcvZH6Yu_1D62VHs_xEf-LMVhsj-kBquscm8UO7OYtgGXr-c)

### 💡 TypeScript Example

```ts
class TreeNode {
  data: number;
  left: TreeNode | null = null;
  right: TreeNode | null = null;

  constructor(data: number) {
    this.data = data;
  }
}

const root = new TreeNode(10);
```

---

# 🔹 GRAPH

## 📘 Overview

👉 Network of nodes and edges

### 🖼️ Visualization

![Image](https://images.openai.com/static-rsc-4/k5Sg-jsZOnNpXq6ZlfzoYVCdwrvO2FQqIPxT0WWXph-Hp4J-UY22F0IzNEsKJ7q76-Y6wL-FFcjOUObpi0UNAS5N8AwqcixfDame7esuh7jEzGDHP4oBMXwEcJhsqOAfNEbCHJ-fPo-wwco-crqmhW2YJVWYi7ndP_F2lRzOrFB58dbvc2ANmkNSuFJorvwj)

### 💡 TypeScript Example

```ts
const graph: Record<string, string[]> = {
  A: ["B", "C"],
  B: ["A"],
};

console.log(graph["A"]);
```

---

# 🎯 Quick Summary

| Structure   | Concept       |
| ----------- | ------------- |
| Array       | Index-based   |
| Linked List | Pointer-based |
| Stack       | LIFO          |
| Queue       | FIFO          |
| Tree        | Hierarchy     |
| Graph       | Network       |

---

```
