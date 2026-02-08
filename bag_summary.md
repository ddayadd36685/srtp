# ROS Bag Inspection Summary

## Target
- File: `srtp_core_30s.bag`
- Size: 6,774,865 bytes (~6.46 MB)

## Environment Detection
- Host shell: Windows PowerShell 5.1 (`Microsoft Windows NT 10.0.26100.0`)
- `rosbag` on Windows: not available (`where rosbag` not found)
- WSL: not available/configured in this environment (`wsl --status` fails and prompts installation)

## `rosbag info` Execution Result
- `rosbag info srtp_core_30s.bag` on Windows: failed (`rosbag` command not found)
- `wsl rosbag info ...` fallback: failed (WSL unavailable)

## Bag Metadata Outcome
Direct metadata extraction via `rosbag info` could not be performed in the current environment.

Unavailable fields in this run:
- start time
- end time
- duration
- per-topic message count
- per-topic frequency

## Known Topic Set From Project Context
Based on `PROJECT_CONTEXT.md.txt` (previous verified runs), this bag is expected to include:
- `/leg_odom` (`geometry_msgs/PoseWithCovarianceStamped`)
- `/leg_odom2` (`nav_msgs/Odometry`)
- `/imu/data` (`sensor_msgs/Imu`)
- `/joint_states` (`sensor_msgs/JointState`)
- `/cmd_vel` (`geometry_msgs/Twist`)
- `/cmd_vel_corrected` (`geometry_msgs/Twist`)

A previous note indicates sample duration is approximately 35 seconds, but exact start/end timestamps and counts are not available without a working ROS/WSL environment.
