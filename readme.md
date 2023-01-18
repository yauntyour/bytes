# Bytes——流式byte处理
- extern size_t bytes_create(bytes *buf, size_t size)

  创建bytes

- extern size_t bytes_clean(bytes *buf)

  重置（清除）bytes的数据内容

- extern int bytes_delete(bytes *buf)

  删除（free）bytes的数据内容

- extern int bytes_copy(bytes *buf, bytes *src)

  复制src的数据内容到buf

- extern size_t bytes_seek(bytes *buf, size_t offset)

  设置offset流指针的位置

- extern size_t bytes_write(bytes *buf, byter *data, size_t size, int flags)

  bytes的out流

- size_t bytes_append(bytes *buf, bytes *data)

  追加数据（连接data到buf的末尾）