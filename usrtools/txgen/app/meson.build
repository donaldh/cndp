# SPDX-License-Identifier: BSD-3-Clause
# Copyright (c) 2019-2022 Intel Corporation

sources = files(
	'cksum.c',
	'cli-functions.c',
	'cmds.c',
	'capture.c',
	'display.c',
	'ether.c',
	'ipv4.c',
	'latency.c',
	'main.c',
	'parse-args.c',
	'_pcap.c',
	'pcap.c',
	'portlist.c',
	'stats.c',
	'tcp.c',
	'txgen.c',
	'udp.c',
	'cne_net_crc.c',
)

deps += [cli, kvargs, pktdev, pktmbuf, mempool, mmap, ring, jcfg, thread, uds, metrics, timer, pmd_af_xdp, pmd_tap, pmd_af_packet, timer, utils]

executable('txgen',
    sources,
    c_args: cflags,
    install: true,
    dependencies: deps)
