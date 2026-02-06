---
created: 2026-02-05 15:07
course: math
tags:
  - study
  - note
  - video-learning
---
Target Deck: math

# Square systems; equations of planes


**📅 日期：** 2026-02-05
**🏫 课程：** [[math]]
**🏷️ 标签：** #study #note

---

## 📺 学习控制台 (Media Extended)
> [!tip] 操作指南
> 1. **右键** 视频链接 -> `Open in Media Extended`
> 2. **Alt+T**：插入时间戳 | **Alt+S**：截图并插入
> 3. **Ctrl+P** -> `Sync with Anki`：一键同步

**视频源：** ![](../../../download/video/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007.mp4)

---

## 📄 参考文档 (PDF)
> [!info] 文档预览
> 如果安装了 **Annotator** 插件，请点击右上角 `More Options` -> `Annotate` 进行批注。

> *本次学习未关联 PDF*

---

## 🧠 核心概念 (Cues)
> *左侧栏：记录关键问题，复习时遮挡右侧*
- [ ] 

## 📝 笔记内容 (Notes)
<% tp.file.cursor() %>

- [00:30](../../../download/video/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007.mp4#t=00:30.37) epquations of plane
- [00:57](../../../download/video/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007.mp4#t=00:57.80) Recall
![](assets/Lec%204_Square%20systems;%20equations%20of%20planes/file-20260206100003168.png)


- [47:52](../../../download/video/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007/Lec%204：%20Square%20systems;%20equations%20of%20planes%20｜%20MIT%2018.02%20Multivariable%20Calculus,%20Fall%202007.mp4#t=47:52.83) general case
- 这是一份基于 MIT 18.02 多变量微积分课程 Lecture 4 讲座内容的详细笔记。

### **MIT 18.02 Lecture 4: 方程组与平面方程 (Square Systems; Equations of Planes)**

本讲座主要探讨了平面的几何方程、线性方程组（特别是 $3\times3$ 系统）的几何解释，以及行列式与解的存在性之间的关系。

---

#### **1. 平面的方程 (Equations of Planes)**

- **一般形式**：平面的方程形式为 $ax + by + cz = d$。
    
- **法向量 (Normal Vector)**：
    
    - 方程中的系数 $\mathbf{(a, b, c)}$ 恰好构成了该平面的**法向量** $\vec{n}$。这是理解平面方程最关键的一点。
    - 方程右边的常数 $d$ 与平面到原点的距离有关（但不完全等于距离，除非法向量是单位向量），它大致衡量了平面相对于原点的平移量。
- **如何求平面方程**：
    
    1. **过原点的平面**：若平面通过原点且法向量为 $\vec{n} = \langle a, b, c \rangle$，则对于平面上任意点 $P(x,y,z)$，向量 $\vec{OP}$ 与 $\vec{n}$ 垂直 ($\vec{OP} \cdot \vec{n} = 0$)。方程为 $ax + by + cz = 0$。
    2. **过特定点 $P_0$ 的平面**：若平面通过点 $P_0$ 且法向量为 $\vec{n}$，则向量 $\vec{P_0P}$ 与 $\vec{n}$ 垂直。方程可以通过代入点 $P_0$ 的坐标来求解常数 $d$。
        - 例如：法向量 $\vec{n}=\langle 1, 5, 10 \rangle$，过点 $P_0(2, 1, -1)$。
        - 方程左边：$x + 5y + 10z$。
        - 代入 $P_0$ 计算右边：$2 + 5(1) + 10(-1) = -3$。
        - 最终方程：$x + 5y + 10z = -3$。

#### **2. 向量与平面的位置关系**

给定一个向量 $\vec{v}$ 和一个平面：

- **垂直**：如果向量 $\vec{v}$ 与平面的法向量 $\vec{n}$ **平行**（成比例），则 $\vec{v}$ 垂直于该平面。
- **平行**：如果向量 $\vec{v}$ 与平面的法向量 $\vec{n}$ **垂直**（即点积 $\vec{v} \cdot \vec{n} = 0$），则 $\vec{v}$ 平行于该平面。

---

#### **3. 线性方程组与几何解释 (Linear Systems and Geometry)**

一个 $3\times3$ 的线性方程组可以看作是三个平面方程的集合。求解方程组等于寻找三个平面的公共交点。

- **几何直观**：
    
    - 前两个方程通常确定两个平面，它们相交于一条**直线**。
    - 第三个方程确定第三个平面。
    - 如果这条直线与第三个平面相交于一点，则系统有**唯一解**。
- **矩阵表示**：
    
    - 方程组写作 $A\mathbf{x} = B$。
    - 如果矩阵 $A$ 可逆，则解为 $\mathbf{x} = A^{-1}B$。

---

#### **4. 解的情况与行列式 (Solutions and Determinants)**

解的存在性取决于系数矩阵 $A$ 的行列式 $\det(A)$。

**情况 A：$\det(A) \neq 0$（非奇异矩阵）**

- 矩阵 $A$ 可逆（存在 $A^{-1}$）。
- 三个平面交于唯一的点。
- 方程组有**唯一解**。

**情况 B：$\det(A) = 0$（奇异矩阵）**

- 矩阵 $A$ 不可逆，不能使用 $A^{-1}B$ 求解。
- **几何意义**：
    - 三个平面的法向量 $\vec{N_1}, \vec{N_2}, \vec{N_3}$ **共面 (Coplanar)**，即它们构成的平行六面体体积为零。
    - 前两个平面交出的直线与第三个平面**平行**。
- **解的可能性**：
    1. **无解 (No Solution)**：前两个平面的交线与第三个平面平行且**不**在其中。会出现如 $0=1$ 的矛盾。
    2. **无穷多解 (Infinitely Many Solutions)**：前两个平面的交线完全**包含**在第三个平面内。会出现如 $0=0$ 的恒等式。整个直线上的点都是解。

---

#### **5. 齐次方程组 (Homogeneous Systems)**

齐次方程组是指右端常数项全为 0 的系统 ($A\mathbf{x} = \mathbf{0}$)。这意味着所有三个平面都经过原点。

- **平凡解 (Trivial Solution)**：原点 $(0,0,0)$ 永远是一个解。
- **解的分类**：
    - 若 $\det(A) \neq 0$：只有唯一的平凡解 $\mathbf{x} = \mathbf{0}$。
    - 若 $\det(A) = 0$：
        - 除了原点外，还有**无穷多非平凡解**。
        - 几何上，交线过原点并包含在所有三个平面内。
        - 交线的方向向量可以通过计算两个法向量的叉积得到：$\vec{v} = \vec{N_1} \times \vec{N_2}$。

---

#### **总结 (Summary)**

| 行列式 $\det(A)$ | $A\mathbf{x}=B$ (一般情况)    | $A\mathbf{x}=\mathbf{0}$ (齐次情况) |
| :------------ | :------------------------ | :------------------------------ |
| **$\neq 0$**  | **唯一解** (点)               | **唯一解** (仅原点 $\mathbf{0}$)      |
| **$= 0$**     | **无解** 或 **无穷多解** (直线或平面) | **无穷多解** (包含原点的直线)              |

---

## 💡 总结 (Summary)
> [!summary] 
> 用一句话总结这篇笔记的核心内容。