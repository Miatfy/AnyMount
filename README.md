
本模块用于在 post-fs-data 阶段将指定目录（如 /odm）挂载到系统根目录，解决部分 ROM 中 overlay 挂载冲突问题。

复制你要挂载的目录（如 /odm）到模块的 anymount/ 文件夹内。
Copy the directories you want to mount (e.g. /odm) to anymount/ to mount them to the root directory at the post-fs-data stage.

刷入模块后重启设备，目录将在系统启动早期自动挂载。
如需挂载多个目录，重复复制操作即可。

注意事项

仅适用于支持 Magisk 的设备，且需已解锁 Bootloader。

刷入前请备份重要数据，避免挂载错误导致系统无法启动。

若更新 ROM（如 OTA 或脏刷），需重新刷入本模块以确保兼容性。 