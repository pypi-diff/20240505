# Comparing `tmp/rlviser_py-0.6.5.tar.gz` & `tmp/rlviser_py-0.6.6.tar.gz`

## Comparing `rlviser_py-0.6.5.tar` & `rlviser_py-0.6.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.5/Cargo.toml
--rw-r--r--   0     1001      127     1070 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/LICENSE
--rw-r--r--   0     1001      127     1557 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/README.md
--rw-r--r--   0     1001      127     2877 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/gym_renderer.py
--rw-r--r--   0     1001      127     2379 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/pygymtest.py
--rw-r--r--   0     1001      127     1030 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/rlviser_py.pyi
--rw-r--r--   0     1001      127    16891 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/src/bytes.rs
--rw-r--r--   0     1001      127     3034 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/src/lib.rs
--rw-r--r--   0     1001      127     2356 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/src/socket.rs
--rw-r--r--   0     1001      127     7861 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/Cargo.lock
--rw-r--r--   0     1001      127      387 2024-04-01 20:23:07.000000 rlviser_py-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 rlviser_py-0.6.6/Cargo.toml
+-rw-r--r--   0     1001      127     1070 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/LICENSE
+-rw-r--r--   0     1001      127     1557 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/README.md
+-rw-r--r--   0     1001      127     2873 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/gym_renderer.py
+-rw-r--r--   0     1001      127     2547 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/pygymtest.py
+-rw-r--r--   0     1001      127     2291 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/rlviser_py.pyi
+-rw-r--r--   0     1001      127    18135 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/src/bytes.rs
+-rw-r--r--   0     1001      127     5195 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/src/lib.rs
+-rw-r--r--   0     1001      127     5462 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/src/socket.rs
+-rw-r--r--   0     1001      127     8092 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/Cargo.lock
+-rw-r--r--   0     1001      127      387 2024-05-05 19:10:45.000000 rlviser_py-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 rlviser_py-0.6.6/PKG-INFO
```

### Comparing `rlviser_py-0.6.5/Cargo.toml` & `rlviser_py-0.6.6/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rlviser-py"
-version = "0.6.5"
+version = "0.6.6"
 edition = "2021"
 description = "Python implementation that manages a UDP connection to RLViser"
 license = "MIT"
 repository = "https://github.com/VirxEC/rlviser-py"
 readme = "README.md"
 keywords = ["rlviser", "rocket-league", "udp", "python", "rlbot"]
 exclude = [".github", "pytest.py", "rustfmt.toml", ".gitignore"]
```

### Comparing `rlviser_py-0.6.5/LICENSE` & `rlviser_py-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.5/README.md` & `rlviser_py-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `rlviser_py-0.6.5/gym_renderer.py` & `rlviser_py-0.6.6/gym_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def render(self, state: GameState, shared_info: Dict[str, Any]) -> Any:
         boost_pad_states = [bool(timer == 0) for timer in state.boost_pad_timers]
 
         ball = rsim.BallState()
         ball.pos = rsim.Vec(*state.ball.position)
         ball.vel = rsim.Vec(*state.ball.linear_velocity)
         ball.ang_vel = rsim.Vec(*state.ball.angular_velocity)
-        ball.rot_mat = rsim.RotMat(*state.ball.rotation_mtx.transpose().flatten())
+        # ball.rot_mat = rsim.RotMat(*state.ball.rotation_mtx.transpose().flatten())
 
         car_data = []
         for idx, car in enumerate(state.cars.values()):
             car_state = self._get_car_state(car)
             car_data.append((idx + 1, car.team_num, rsim.CarConfig(car.hitbox_type), car_state))
 
         self.packet_id += 1
@@ -55,15 +55,15 @@
         car_state.is_jumping = car.is_jumping
         car_state.jump_time = car.jump_time
 
         car_state.has_flipped = car.has_flipped
         car_state.has_double_jumped = car.has_double_jumped
         car_state.air_time_since_jump = car.air_time_since_jump
         car_state.flip_time = car.flip_time
-        car_state.last_rel_dodge_torque = rsim.Vec(*car.flip_torque)
+        car_state.flip_rel_torque = rsim.Vec(*car.flip_torque)
 
         car_state.is_auto_flipping = car.is_autoflipping
         car_state.auto_flip_timer = car.autoflip_timer
         car_state.auto_flip_torque_scale = car.autoflip_direction
 
         if car.bump_victim_id is not None:
             car_state.car_contact_id = car.bump_victim_id
```

### Comparing `rlviser_py-0.6.5/pygymtest.py` & `rlviser_py-0.6.6/pygymtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 import time
-import numpy as np
 from itertools import chain
 
+import numpy as np
+import rlviser_py
 from rlgym.api import RLGym
 from rlgym.rocket_league.action_parsers import LookupTableAction, RepeatAction
-from rlgym.rocket_league.done_conditions import GoalCondition, AnyCondition, TimeoutCondition, NoTouchTimeoutCondition
+from rlgym.rocket_league.done_conditions import (
+    AnyCondition,
+    GoalCondition,
+    NoTouchTimeoutCondition,
+    TimeoutCondition,
+)
 from rlgym.rocket_league.obs_builders import DefaultObs
 from rlgym.rocket_league.reward_functions import CombinedReward, GoalReward, TouchReward
 from rlgym.rocket_league.sim import RocketSimEngine
-from rlgym.rocket_league.state_mutators import MutatorSequence, FixedTeamSizeMutator, KickoffMutator
+from rlgym.rocket_league.state_mutators import (
+    FixedTeamSizeMutator,
+    KickoffMutator,
+    MutatorSequence,
+)
 
 from gym_renderer import RLViserRenderer
 
 if __name__ == "__main__":
+    game_speed = 1
+
     env = RLGym(
         state_mutator=MutatorSequence(
-            FixedTeamSizeMutator(blue_size=2, orange_size=2),
-            KickoffMutator()
+            FixedTeamSizeMutator(blue_size=2, orange_size=2), KickoffMutator()
         ),
         obs_builder=DefaultObs(zero_padding=None),
         action_parser=RepeatAction(LookupTableAction(), repeats=1),
-        reward_fn=CombinedReward(
-            (GoalReward(), 10.),
-            (TouchReward(), 0.1)
-        ),
+        reward_fn=CombinedReward((GoalReward(), 10.0), (TouchReward(), 0.1)),
         termination_cond=GoalCondition(),
         truncation_cond=AnyCondition(
-            TimeoutCondition(timeout=300.),
-            NoTouchTimeoutCondition(timeout=30.)
+            TimeoutCondition(timeout=300.0), NoTouchTimeoutCondition(timeout=30.0)
         ),
         transition_engine=RocketSimEngine(),
-        renderer=RLViserRenderer(120)
+        renderer=RLViserRenderer(120),
     )
 
     # simulate 2 episodes
     for _ in range(2):
         obs_dict = env.reset()
         steps = 0
-        ep_reward = {agent_id: 0. for agent_id in env.agents}
+        ep_reward = {agent_id: 0.0 for agent_id in env.agents}
         t0 = time.time()
         while True:
             actions = {}
             for agent_id, action_space in env.action_spaces.items():
                 # agent.act(obs) | Your agent should go here
                 actions[agent_id] = np.random.randint(action_space, size=(1,))
 
             for _ in range(8):
-                obs_dict, reward_dict, terminated_dict, truncated_dict = env.step(actions)
+                obs_dict, reward_dict, terminated_dict, truncated_dict = env.step(
+                    actions
+                )
                 env.render()
-                time.sleep(max(0, t0 + steps / 1200 - time.time()))
+                time.sleep(max(0, t0 + steps / (120 * game_speed) - time.time()))
                 steps += 1
 
             for agent_id, reward in reward_dict.items():
                 ep_reward[agent_id] += reward
 
             if any(chain(terminated_dict.values(), truncated_dict.values())):
                 break
 
+            game_speed = rlviser_py.get_game_speed()
+
         ep_time = time.time() - t0
-        print(f"Steps per second: {steps / ep_time:.0f} | Episode time: {ep_time:.2f} | Episode Reward: {max(ep_reward.values()):.2f}")
+        print(
+            f"Steps per second: {steps / ep_time:.0f} | Episode time: {ep_time:.2f} | Episode Reward: {max(ep_reward.values()):.2f}"
+        )
+
+    env.close()
```

### Comparing `rlviser_py-0.6.5/src/bytes.rs` & `rlviser_py-0.6.6/src/bytes.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use core::fmt;
 use pyo3::FromPyObject;
 
 #[repr(u8)]
 #[derive(Clone, Copy, Debug, Default)]
 pub enum GameMode {
     Soccar,
     Hoops,
@@ -94,19 +95,19 @@
     pub extra_hit_vel: Vec3,
     pub tick_count_when_hit: u64,
     pub tick_count_when_extra_impulse_applied: u64,
 }
 
 #[derive(Clone, Copy, Debug, FromPyObject)]
 pub struct BallState {
-    pub update_counter: u64,
     pub pos: Vec3,
     pub rot_mat: RotMat,
     pub vel: Vec3,
     pub ang_vel: Vec3,
+    pub update_counter: u64,
     pub heatseeker_target_dir: f32,
     pub heatseeker_target_speed: f32,
     pub heatseeker_time_since_hit: f32,
 }
 
 pub type TBall = (TVec3, TRotMat, TVec3, TVec3);
 
@@ -183,24 +184,25 @@
     pub boost: bool,
     pub jump: bool,
     pub handbrake: bool,
 }
 
 #[derive(Clone, Copy, Debug, Default, FromPyObject)]
 pub struct CarState {
-    pub update_counter: u64,
     pub pos: Vec3,
     pub rot_mat: RotMat,
     pub vel: Vec3,
     pub ang_vel: Vec3,
+    pub update_counter: u64,
     pub is_on_ground: bool,
+    pub wheels_with_contact: [bool; 4],
     pub has_jumped: bool,
     pub has_double_jumped: bool,
     pub has_flipped: bool,
-    pub last_rel_dodge_torque: Vec3,
+    pub flip_rel_torque: Vec3,
     pub jump_time: f32,
     pub flip_time: f32,
     pub is_flipping: bool,
     pub is_jumping: bool,
     pub air_time_since_jump: f32,
     pub boost: f32,
     pub time_spent_boosting: f32,
@@ -295,14 +297,15 @@
     pub fn read<I: FromBytesExact>(&mut self) -> I {
         let item = I::from_bytes(&self.bytes[self.idx..self.idx + I::NUM_BYTES]);
         self.idx += I::NUM_BYTES;
         item
     }
 
     #[inline]
+    #[track_caller]
     pub fn debug_assert_num_bytes(&self, num_bytes: usize) {
         debug_assert_eq!(self.idx, num_bytes, "ByteReader::debug_assert_num_bytes() failed");
     }
 }
 
 impl FromBytes for bool {
     #[inline]
@@ -322,14 +325,36 @@
 impl FromBytes for f32 {
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
         Self::from_le_bytes([bytes[0], bytes[1], bytes[2], bytes[3]])
     }
 }
 
+impl FromBytesExact for u8 {
+    const NUM_BYTES: usize = 1;
+}
+
+impl FromBytes for u8 {
+    #[inline]
+    fn from_bytes(bytes: &[u8]) -> Self {
+        bytes[0]
+    }
+}
+
+impl FromBytesExact for u16 {
+    const NUM_BYTES: usize = 2;
+}
+
+impl FromBytes for u16 {
+    #[inline]
+    fn from_bytes(bytes: &[u8]) -> Self {
+        Self::from_le_bytes([bytes[0], bytes[1]])
+    }
+}
+
 impl FromBytesExact for u32 {
     const NUM_BYTES: usize = 4;
 }
 
 impl FromBytes for u32 {
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
@@ -344,14 +369,39 @@
 impl FromBytes for u64 {
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
         Self::from_le_bytes([bytes[0], bytes[1], bytes[2], bytes[3], bytes[4], bytes[5], bytes[6], bytes[7]])
     }
 }
 
+impl FromBytesExact for i32 {
+    const NUM_BYTES: usize = 4;
+}
+
+impl FromBytes for i32 {
+    #[inline]
+    fn from_bytes(bytes: &[u8]) -> Self {
+        Self::from_le_bytes([bytes[0], bytes[1], bytes[2], bytes[3]])
+    }
+}
+
+impl<T: FromBytesExact + fmt::Debug, const N: usize> FromBytesExact for [T; N] {
+    const NUM_BYTES: usize = T::NUM_BYTES * N;
+}
+
+impl<T: FromBytesExact + fmt::Debug, const N: usize> FromBytes for [T; N] {
+    fn from_bytes(bytes: &[u8]) -> Self {
+        let mut reader = ByteReader::new(bytes);
+
+        let items = (0..N).map(|_| reader.read()).collect::<Vec<T>>();
+        reader.debug_assert_num_bytes(Self::NUM_BYTES);
+        items.try_into().unwrap()
+    }
+}
+
 impl FromBytesExact for Team {
     const NUM_BYTES: usize = 1;
 }
 
 impl FromBytes for Team {
     #[inline]
     fn from_bytes(bytes: &[u8]) -> Self {
@@ -434,49 +484,47 @@
     #[inline]
     pub fn inner(self) -> [u8; N] {
         debug_assert_eq!(self.idx, N, "ByteWriter::inner() called before all bytes were written");
         self.bytes
     }
 }
 
-impl ToBytesExact<{ Self::NUM_BYTES }> for bool {
-    fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
-        [u8::from(*self)]
-    }
-}
-
-impl ToBytesExact<{ Self::NUM_BYTES }> for u32 {
-    fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
-        self.to_le_bytes()
+impl ToBytesExact<{ bool::NUM_BYTES * 4 }> for [bool; 4] {
+    fn to_bytes(&self) -> [u8; bool::NUM_BYTES * 4] {
+        let mut writer = ByteWriter::<{ bool::NUM_BYTES * 4 }>::new();
+        for item in self {
+            writer.write(item);
+        }
+        writer.inner()
     }
 }
 
-impl ToBytesExact<{ Self::NUM_BYTES }> for u64 {
-    fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
-        self.to_le_bytes()
-    }
+macro_rules! impl_to_bytes_exact_via_std {
+    ($($t:ty),+) => {
+        $(impl ToBytesExact<{ Self::NUM_BYTES }> for $t {
+            fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
+                self.to_le_bytes()
+            }
+        })+
+    };
 }
 
-impl ToBytesExact<{ Self::NUM_BYTES }> for f32 {
-    fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
-        self.to_le_bytes()
-    }
-}
+impl_to_bytes_exact_via_std!(u8, u16, u32, u64, i32, f32);
 
-impl ToBytesExact<{ Self::NUM_BYTES }> for Team {
-    fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
-        [*self as u8]
-    }
+macro_rules! impl_to_bytes_exact_as_u8 {
+    ($($t:ty),+) => {
+        $(impl ToBytesExact<{ Self::NUM_BYTES }> for $t {
+            fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
+                [*self as u8]
+            }
+        })+
+    };
 }
 
-impl ToBytesExact<{ Self::NUM_BYTES }> for GameMode {
-    fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
-        [*self as u8]
-    }
-}
+impl_to_bytes_exact_as_u8!(bool, Team, GameMode);
 
 macro_rules! impl_to_bytes_exact {
     ($t:ty, $($p:ident),+) => {
         impl ToBytesExact<{ Self::NUM_BYTES }> for $t {
             fn to_bytes(&self) -> [u8; Self::NUM_BYTES] {
                 let mut writer = ByteWriter::<{ Self::NUM_BYTES }>::new();
                 $(writer.write(&self.$p);)+
@@ -546,29 +594,30 @@
     handbrake
 );
 impl_bytes_exact!(
     CarState,
     u64::NUM_BYTES
         + Vec3::NUM_BYTES * 5
         + RotMat::NUM_BYTES
-        + 10
-        + f32::NUM_BYTES * 11
+        + 14
+        + f32::NUM_BYTES * 12
         + u32::NUM_BYTES
         + BallHitInfo::NUM_BYTES
         + CarControls::NUM_BYTES,
     update_counter,
     pos,
     rot_mat,
     vel,
     ang_vel,
     is_on_ground,
+    wheels_with_contact,
     has_jumped,
     has_double_jumped,
     has_flipped,
-    last_rel_dodge_torque,
+    flip_rel_torque,
     jump_time,
     flip_time,
     is_flipping,
     is_jumping,
     air_time_since_jump,
     boost,
     time_spent_boosting,
```

### Comparing `rlviser_py-0.6.5/Cargo.lock` & `rlviser_py-0.6.6/Cargo.lock`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -30,23 +30,23 @@
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.154"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "ae743338b92ff9146ce83992f766a31066a91a8c84a45e0e9f21e7cf6de6d346"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
@@ -61,27 +61,27 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
@@ -90,26 +90,26 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -117,78 +117,78 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rlviser-py"
-version = "0.6.5"
+version = "0.6.6"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
@@ -199,17 +199,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.57"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -228,61 +228,68 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
+ "windows_i686_gnullvm",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `rlviser_py-0.6.5/PKG-INFO` & `rlviser_py-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rlviser-py
-Version: 0.6.5
+Version: 0.6.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python implementation that manages a UDP connection to RLViser
 Keywords: rlviser,rocket-league,udp,python,rlbot
 License: MIT
```

