# Derek Poe

I build infrastructure software and investigate performance across runtimes, operating systems, devices, and networks. My background combines software development, infrastructure operations, and a Doctor of Computer Science in Big Data Analytics.

My work centers on concurrency, observability, and understanding how a system behaves from input to output.

## Selected systems

### [PSAccel](https://github.com/Derek-Poe/PSAccel)

A GPU filtering framework for PowerShell using C#, runtime-generated HLSL, and Direct3D 11 compute shaders. I built the interop and filtering pipeline and evaluated GPU-accelerated filtering in my doctoral research.

Engineering focus: data representation, CPU-to-GPU transfer, shader dispatch, synchronization, result readback, and experimental design.

### [yPad](https://github.com/Derek-Poe/yPad)

A Rust and Objective-C streaming system that connects a Linux-hosted Android environment to legacy iOS hardware. It combines Waydroid/Wayland capture, H.264 over RTP, hardware decoding, and an input return path.

Engineering focus: bounded buffering, stale-frame dropping, independent media and control paths, and diagnostics across the capture, encode, network, decode, and render stages.

### [IPUAPI](https://github.com/Derek-Poe/IPUAPI)

A PowerShell web management system built around a reverse-engineered binary UDP command protocol. I used Wireshark packet analysis to reconstruct command layouts, insert device-specific parameters, and support reporting-rate changes and firmware operations. The published package extracts the command builders and job-state logic into an offline, tested module with synthetic identifiers; it includes sanitized historical references to the original server.

Engineering focus: protocol interoperability, queued operations, verification against reported device state, and process watchdogs.

### [SitebossHub](https://github.com/Derek-Poe/SitebossHub)

A sensor-monitoring dashboard originally backed by PowerShell collectors, packaged with a synthetic FastAPI backend. The browser UI includes Canvas sparklines, sensor drill-down, history, alarms, and generator-run views.

I built the first version to support Hurricane Laura recovery. A help desk/admin team used it daily to monitor 34 fixed cell tower sites and two mobile sites, including periods of 24/7 team coverage. [Collector workflow and deployment context](https://github.com/Derek-Poe/SitebossHub/blob/main/docs/collector-case-study.md).

Engineering focus: stable collector/UI contracts, bounded history, deterministic simulation, concurrent access, and observable system state.

## Inspect and reproduce

| Project | Start here | Evidence and scope |
| --- | --- | --- |
| PSAccel | [Current benchmark and CPU comparison](https://github.com/Derek-Poe/PSAccel/tree/main/benchmark/current) | Exact-result checks, raw current measurements, a specialized CPU baseline, and a separately identified historical study |
| yPad | [Recorded software demo](https://github.com/Derek-Poe/yPad/blob/main/docs/demo/README.md) | Synthetic RTP streaming, independent video decoding, browser playback/reconnect, and audio resampling checks; physical-device demo pending setup |
| IPUAPI | [Offline protocol examples](https://github.com/Derek-Poe/IPUAPI#readme) | Packet fixtures and job-state checks without sending commands to devices |
| SitebossHub | [Run the dashboard](https://github.com/Derek-Poe/SitebossHub#run-locally) | Synthetic monitoring data, API tests, and browser checks; the original production collectors are separate |

## Further engineering work

- [PowerShell Request Engine](https://github.com/Derek-Poe/PowerShell-RequestEngine) modernizes my CRM server's scheduler with bounded admission, isolated runspaces, deadlines, and cooperative cancellation.
- [Ensemble3D](https://github.com/Derek-Poe/Ensemble3D) extracts my 3D workbench's local job and asset pipeline to demonstrate SQLite transaction correctness, immutable versions, and detection of interrupted work.
- [E3P Studio](https://github.com/Derek-Poe/E3PStudio) extracts my toolpath transformation work into an offline geometry demo with state-preservation tests and reproducible synthetic visuals.

## Background

I have worked across production software, data systems, infrastructure administration, and communications electronics. I am a former Marine Corps Sergeant and completed my DCS at Colorado Technical University in 2026.

Languages and platforms I use include C#, PowerShell, Rust, Python, JavaScript, Linux, Windows, Direct3D, and TCP/UDP networking.
