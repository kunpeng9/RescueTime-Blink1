营救时间-blink1
=================

一个示例脚本演示如何使用闪烁(1)状态灯显示当前营救时间生产率脉冲。

效率脉动是你在 RescueTime 中记录的所有活动的平均得分，基于应用到它们的效率水平。

# # 使用这个脚本

你需要在你的系统上安装 Ruby，并安装‘ blink1’ gem-[点击这里]( https://rubygems.org/gems/blink1文件夹)

1. 复制文件 rescuetime api key template. rb，并将其重命名为 rescuetime api key. rb
2. 在 RescueTime _ API _ key. rb’中，更新‘ API _ key’值以使用有效的 RescueTime API 键-[更多信息]( https://www.RescueTime.com/anapi/manage )
3. 插上你的闪光灯(1)如果它还没有亮起来
图4。在终端机上，呼叫“救援时间”。Rb 脚本更新 Blink (1)的颜色，以反映您当前的生产力脉搏。(有关连续轮询的更多信息，请参阅下面的“轮询 api”部分)

# # 轮询 API

呼救时间到了。Rb’脚本将更新光一次。要让它连续运行，可以使用操作系统的调度工具(例如 Cron) ，或者打开终端窗口并使用下面的命令:

‘ while true; do ruby ~/YOUR/PATH/TO/thingm-rescuetime/thingm-rescuetime. rb; sleep 180; clear; done’

使用此方法时，可以键入“ CTRL + c”退出循环，或者完成后关闭终端窗口。

* 注意: RescueTime 在 MAXIMUM 每三分钟更新一次，所以频繁的轮询没有任何意义。*

还有一个方便的脚本——“ thingm-off. rb”——用来关灯。
-
RescueTime-Blink1
=================

An example script to show how to use a Blink(1) Status Light do display your current RescueTime productivity pulse.

The productivity pulse is an average score of all the activities you've logged time for in RescueTime, based on the productivity levels that have been applied to them.

## To use this script

You will need to have Ruby on your system, and install the `blink1` gem - [Get it here](https://rubygems.org/gems/blink1)

1. Make a copy of the file `rescuetime_api_key_TEMPLATE.rb` and rename it to `rescuetime_api_key.rb`
2. In `rescuetime_api_key.rb`, update the `API_KEY` value to use a valid RescueTime API key - [More info](https://www.rescuetime.com/anapi/manage)
3. Plug in your Blink(1) Light if it's not already
4. In a terminal, call the `thingm-rescuetime.rb` script to update the Blink(1)'s color to reflect your current productivity pulse. (see 'polling the api' section below for more about continuous polling')

## Polling the API

Calling the `thingm-rescuetime.rb` script will update the light a single time. To have it run continuously, use your operating system's scheduling utility (Cron, for example), or open a terminal window and use a command like this:

`while true ; do ruby ~/YOUR/PATH/TO/thingm-rescuetime/thingm-rescuetime.rb ; sleep 180 ; clear ; done`

When using this method, you can type `CTRL+c` to exit the loop, or just close the terminal window when you're done.

*NOTE: RescueTime updates at the MAXIMUM every three minutes, so it doesn't make any sense to poll more frequently than that.*

There is also a convenience script included - `thingm-off.rb` - to shut the light off.
