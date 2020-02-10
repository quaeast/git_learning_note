# Linux 安装二进制 Node

```bash
# 从 https://nodejs.org/en/download/ 下载软件
wget https://nodejs.org/dist/v12.15.0/node-v12.15.0-linux-x64.tar.xz

# 解压
tar -xJvf node-v12.15.0-linux-x64.tar.xz

# 移动
mv node-v12.15.0-linux-x64 /usr/local/lib

# 在 ~/.bashrc 或 ~/.zshrc 中添加环境变量
export NODE_HOME=/usr/local/lib/node-v12.15.0-linux-x64
export PATH=$NODE_HOME/bin:$PATH
```

## 附录

### 1

usr 不是user缩写，而是，`unix system resource` 缩写.
其中, `/lib`是内核级的, `/usr/lib`是系统级的, `/usr/local/lib`是用户级的.

### 2

`.xz` 使用参数 `-J` 进行解压
`.gz` 使用参数 `-z` 进行解压