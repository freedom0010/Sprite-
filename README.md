# Sprite-
模拟真实用户打字：字母识别准确率 60%，40% 概率输入错误字符。
错误字符有 80% 概率被更正，模拟人类打字和修正行为。
按键间隔随机化（50-150ms），模拟自然打字节奏。

模拟鼠标轨迹移动、随机晃动、点击：在点击前模拟鼠标轨迹移动，包含随机偏移。
20% 概率触发随机鼠标晃动，模拟无意识行为。
点击事件包含 mouseover, mousedown, mouseup, click，并添加随机延迟。

防检测：窗口失焦：10% 概率触发失焦并重新聚焦，模拟人类分心。
点击节奏：所有点击和输入操作使用随机延迟（20-1000ms），避免规律性模式。
滚动行为：20% 概率触发随机页面滚动，模拟浏览行为。

模块化结构：将功能拆分为模块（如输入、鼠标操作、状态管理），提高代码可维护性。
支持配置轮数和得分上限，通过参数控制脚本行为。

暂停/恢复/中断：添加全局状态管理，支持暂停、恢复和中断脚本。
提供控制函数（如 pauseScript, resumeScript, stopScript），可通过控制台调用。

