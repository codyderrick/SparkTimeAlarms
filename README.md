SparkTimeAlarms
===============

Port of PJRC's TimeAlarms Library using core Time.now

Please note that this library is not intended to work with the SparkTime NTP library.

This library only works with built-in core Time.now() initialized from the Spark Cloud.

Note the Alarm.delay(1000) in the example -  Alarm.delay must be used
instead of the usual Particle delay function because the alarms are serviced in the Alarm.delay method.
Failing to regularly call Alarm.delay will result in the alarms not being triggered
so always use Alarm.delay instead of delay in sketches that use the Alarms library.
