# PartiallyObservableGym
This repository summarizes tasks used in DRL and defines a set of POMDP on top of them.

<table style="height: 225px; width: 616px;">
<tbody>
<tr>
<td style="width: 65px; text-align: center;" rowspan="2">Platform</td>
<td style="width: 218px; text-align: center;" colspan="2" rowspan="2">Task</td>
<td style="width: 335px; text-align: center;" colspan="2">Observation</td>
<td style="width: 54px; text-align: center;" colspan="2">Action</td>
</tr>
<tr>
<td style="width: 28px; text-align: center;">Dim</td>
<td style="width: 307px; text-align: center;" rowspan="1">Comp</td>
<td style="width: 10px; text-align: center;">Dim</td>
<td style="width: 44px; text-align: center;" rowspan="1">Comp</td>
</tr>
<tr>
<td style="width: 65px; text-align: center;" rowspan="22">&nbsp;OpenAI Gym</td>
<td style="width: 66px;" rowspan="22">&nbsp;MuJoCo</td>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/half_cheetah_v3.py" target="_blank" rel="noopener">HalfCheetah-v3</a> <a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/half_cheetah.py" target="_blank" rel="noopener">HalfCheetah-v2</a></td>
<td style="width: 28px; text-align: center;">17</td>
<td style="width: 307px; text-align: center;">
<ul>
<li style="text-align: left;">Position: 1-8 (d=8)</li>
<li style="text-align: left;">Velocity: 9-17 (d=9)</li>
</ul>
</td>
<td style="width: 10px; text-align: center;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/ant_v3.py" target="_blank" rel="noopener">Ant-v3</a> <a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/ant.py" target="_blank" rel="noopener">Ant-v2</a></td>
<td style="width: 28px;">111</td>
<td style="width: 307px;">
<ul>
<li>position: 1-13 (d=13)</li>
<li>velocity: 14-27 (d=14)</li>
<li>cfrc_ext: 28-111 (d=64)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 10px;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/walker2d_v3.py" target="_blank" rel="noopener">Walker2d-v3</a> <a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/walker2d.py" target="_blank" rel="noopener">Walker2d-v2</a></td>
<td style="width: 28px;">&nbsp;17</td>
<td style="width: 307px;">
<ul>
<li>position: 1-8 (d=8)</li>
<li>velocity: 9-17 (d=9)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px;">&nbsp;<a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/hopper_v3.py" target="_blank" rel="noopener">Hopper-v3</a>&nbsp;<a href="http://localhost:8888/notebooks/Google%20Drive/git_repos/spinningup-new/spinup/algos/pytorch/lstm_ddpg/Untitled2.ipynb" target="_blank" rel="noopener">Hopper-v2</a></td>
<td style="width: 28px;">&nbsp;11</td>
<td style="width: 307px;">
<ul>
<li>&nbsp;position: 1-5 (d=5)</li>
<li>velocity: 6-11 (d=6)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/inverted_pendulum.py" target="_blank" rel="noopener">InvertedPendulum-v2</a></td>
<td style="width: 28px;">4</td>
<td style="width: 307px;">
<ul>
<li>position: 1-2 (d=2)</li>
<li>velocity: 3-4 (d=2)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/inverted_double_pendulum.py" target="_blank" rel="noopener">InvertedDoublePendulum-v2</a></td>
<td style="width: 28px;">11</td>
<td style="width: 307px;">
<ul>
<li>cart position: 1</li>
<li>link angles sin: 2-3</li>
<li>link angles cos: 4-5</li>
<li>link velocity: 6-8 (d=3)</li>
<li>qfrc_constraint: 9-11 (d=3)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/swimmer_v3.py" target="_blank" rel="noopener">Swimmer-v3</a>&nbsp;<a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/walker2d.py" target="_blank" rel="noopener">Swimmer-v2</a></td>
<td style="width: 28px;">8</td>
<td style="width: 307px;">
<ul>
<li>position: 1-3 (d=3)</li>
<li>velocity: 4-8 (d=5)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/thrower.py" target="_blank" rel="noopener">Thrower-v2</a></td>
<td style="width: 28px;">23</td>
<td style="width: 307px;">
<ul>
<li>position: 1-7 (d=7)</li>
<li>velocity: 8-14 (d=7)</li>
<li>get_body_com("r_wrist_roll_link"): 15-17 (d=3)</li>
<li>get_body_com("ball"): 18-20 (d=3)</li>
<li>get_body_com("goal"): 21-23 (d=3)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/striker.py" target="_blank" rel="noopener">Striker-v2</a></td>
<td style="width: 28px;">23</td>
<td style="width: 307px;">
<ul>
<li>position: 1-7 (d=7)</li>
<li>velocity: 8-14 (d=7)</li>
<li>get_body_com("tips_arm"): 15-17 (d=3)</li>
<li>get_body_com("object"): 18-20 (d=3)</li>
<li>get_body_com("goal"): 21-23 (d=3)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/pusher.py" target="_blank" rel="noopener">Pusher-v2</a></td>
<td style="width: 28px;">23</td>
<td style="width: 307px;">
<ul>
<li>position: 1-7 (d=7)</li>
<li>velocity: 8-14 (d=7)</li>
<li>get_body_com("tips_arm"): 15-17 (d=3)</li>
<li>get_body_com("object"): 18-20 (d=3)</li>
<li>get_body_com("goal"): 21-23 (d=3)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/reacher.py" target="_blank" rel="noopener">Reacher-v2</a></td>
<td style="width: 28px;">11</td>
<td style="width: 307px;">
<ul>
<li>cos: 1-2 (d=2)</li>
<li>sin: 3-4 (d=2)</li>
<li>position: 5-6 (d=2)</li>
<li>velocity: 7-8 (d=2)</li>
<li>get_body_com("fingertip")-get_body_com("target"): 9-11 (d=3)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/humanoid_v3.py" target="_blank" rel="noopener">Humanoid-v3</a>&nbsp;<a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/humanoid.py" target="_blank" rel="noopener">Humanoid-v2</a></td>
<td style="width: 28px;">376</td>
<td style="width: 307px;">
<ul>
<li>position: 1-22 (d=22)</li>
<li>velocity: 23-45 (d=23)</li>
<li>com_inertia: 46-185 (d=140)</li>
<li>com_velocity: 186-269 (d=84)</li>
<li>actuator_forces: 270-292 (d=23)</li>
<li>external_contact_forces: 293-376 (d=84)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
<tr>
<td style="width: 152px; text-align: center;"><a href="https://github.com/openai/gym/blob/master/gym/envs/mujoco/humanoidstandup.py" target="_blank" rel="noopener">HumanoidStandup-v2</a></td>
<td style="width: 28px;">376</td>
<td style="width: 307px;">
<ul>
<li>position: 1-22 (d=22)</li>
<li>velocity: 23-45 (d=23)</li>
<li>com_inertia: 46-185 (d=140)</li>
<li>com_velocity: 186-269 (d=84)</li>
<li>actuator_forces: 270-292 (d=23)</li>
<li>external_contact_forces: 293-376 (d=84)</li>
</ul>
</td>
<td style="width: 10px;">&nbsp;</td>
<td style="width: 44px; text-align: center;">&nbsp;</td>
</tr>
</tbody>
</table>
