# The-Book-Nook
这个项目是刚接触计算机时写的增删改查（c++是真难绷）！真希望这段代码是我和C语言的告别~

## 文件结构

本项目包含三个文件：

* `workermanager.h`: 头文件，包含 `WorkerManager` 类的声明。
* `workermanager.cpp`: 源文件，包含 `WorkerManager` 类的实现。
* `main.cpp`: 源文件，包含程序入口函数 `main`。

## WorkerManager 类

`WorkerManager` 类负责管理员工信息，提供以下功能：

```cpp
class WorkerManager {
public:
    void Show_Menu(); // 显示菜单
    void Exit_System(); // 退出程序
    void Add_Emp(); // 添加职工
    void save(); // 保存信息
    bool m_File_Is_Empty; // 判断文件是否为空
    void init_Emp(); // 初始化员工
    void Show_Emp(); // 显示员工
    void Del_Emp(); // 删除员工
    void Mod_Emp(); // 修改员工
    void File_Emp(); // 查找员工
    void Sort_Emp(); // 排序
    void Clean_File(); // 清理文档
};
```

## 可视化：
```txt
Welcome to the employee management systom!
0. Exit the management program
1. Add employee information
2. Display employee information
3. Delete job-hopping employees
4. Modify employee information
5. Find employee information
6. Sort by number
7. Clear all documentsy

```
## 代码复用

将 `WorkerManager` 类的声明放在头文件中，方便在多个源文件中调用，提高了代码的复用性。

## 代码维护

将 `WorkerManager` 类的实现放在单独的源文件中，使得代码结构更加清晰，便于修改和维护。
