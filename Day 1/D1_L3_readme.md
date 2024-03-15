### Get familiar to open-source EDA tools
<details>
  <summary>Whole File Structure of OpenLane</summary>
  
├── AUTHORS.md
├── clean_runs.tcl
├── configuration
│   ├── checkers.tcl
│   ├── cts.tcl
│   ├── floorplan.tcl
│   ├── general.tcl
│   ├── lvs.tcl
│   ├── placement.tcl
│   ├── README.md
│   ├── routing.tcl
│   └── synthesis.tcl
├── conf.py
├── CONTRIBUTING.md
├── default.cvcrc
├── designs
│   ├── 151
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── ALUdec.v
│   │       ├── ALUop.vh
│   │       ├── ALU.v
│   │       ├── backup_mem.v
│   │       ├── Cache.v
│   │       ├── const.vh
│   │       ├── controller.v
│   │       ├── datapath.v
│   │       ├── DataSRAMs.v
│   │       ├── ExecuteStage.v
│   │       ├── FetchDecodeStage.v
│   │       ├── Memory141.v
│   │       ├── no_cache_mem.v
│   │       ├── Opcode.vh
│   │       ├── RegisterFile.v
│   │       ├── Riscv141.v
│   │       ├── riscv_arbiter.v
│   │       ├── riscv_top.v
│   │       ├── TagSRAMs.v
│   │       └── WriteBackStage.v
│   ├── aes
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── aes_core.sdc
│   │       ├── aes.sdc
│   │       └── aes.v
│   ├── aes128
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── aes128.sdc
│   │       └── aes128.v
│   ├── aes192
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── aes192.sdc
│   │       └── aes192.v
│   ├── aes256
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── aes256.sdc
│   │       └── aes256.v
│   ├── aes_cipher
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── aes_cipher.v
│   │       ├── aes_key_expand_128.v
│   │       ├── aes_rcon.v
│   │       ├── aes_sbox.v
│   │       ├── aes.v.x
│   │       └── timescale.v
│   ├── aes_core
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── aes_core.sdc
│   │       ├── aes_core.v
│   │       ├── aes.sdc
│   │       └── aes.v
│   ├── APU
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── APU.v
│   ├── blabla
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── blabla.sdc
│   │       └── blabla.v
│   ├── BM64
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── BM64.sdc
│   │       └── BM64.v
│   ├── chacha
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── chacha.sdc
│   │       └── chacha.v
│   ├── cic_decimator
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── cic_decimator.v
│   ├── des
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── 3des.v
│   │       └── des.sdc
│   ├── des3
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── 3des.v
│   │       └── des3.sdc
│   ├── digital_pll_sky130_fd_sc_hd
│   │   ├── config.tcl
│   │   └── src
│   │       ├── digital_pll_controller.v
│   │       ├── digital_pll.v
│   │       └── ring_osc2x13.v
│   ├── genericfir
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── genericfir.sdc
│   │       └── genericfir.v
│   ├── inverter
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── inverter.v
│   ├── jpeg_encoder
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── dct_cos_table.v
│   │       ├── dct_mac.v
│   │       ├── dctub.v
│   │       ├── dctu.v
│   │       ├── dct.v
│   │       ├── div_su.v
│   │       ├── div_uu.v
│   │       ├── fdct.v
│   │       ├── jpeg_encoder.v
│   │       ├── jpeg_qnr.v
│   │       ├── jpeg_rle1.v
│   │       ├── jpeg_rle.v
│   │       ├── jpeg_rzs.v
│   │       ├── jpeg.v
│   │       └── zigzag.v
│   ├── ldpc_decoder_802_3an
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── ldpc_decoder_802_3an.v
│   ├── ldpcenc
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── ldpcenc.v
│   ├── manual_macro_placement_test
│   │   ├── config.tcl
│   │   ├── macro_placement.cfg
│   │   ├── macros
│   │   │   ├── gds
│   │   │   │   └── spm.gds
│   │   │   └── lef
│   │   │       └── spm.lef
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── design.v
│   ├── md5
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── md5.sdc
│   │       └── md5.v
│   ├── ocs_blitter
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── ocs_blitter.v
│   ├── picorv32a
│   │   ├── config.tcl
│   │   ├── runs
│   │   │   └── 14-03_06-18
│   │   │       ├── cmds.log
│   │   │       ├── config.tcl
│   │   │       ├── logs
│   │   │       │   ├── 0-prep_runtime.txt
│   │   │       │   ├── cts
│   │   │       │   ├── cvc
│   │   │       │   ├── floorplan
│   │   │       │   ├── flow_summary.log
│   │   │       │   ├── klayout
│   │   │       │   ├── lvs
│   │   │       │   ├── magic
│   │   │       │   ├── placement
│   │   │       │   ├── routing
│   │   │       │   └── synthesis
│   │   │       │       ├── 1-yosys.log
│   │   │       │       ├── 1-yosys_runtime.txt
│   │   │       │       ├── 2-opensta
│   │   │       │       └── 2-opensta_runtime.txt
│   │   │       ├── OPENLANE_VERSION
│   │   │       ├── PDK_SOURCES
│   │   │       ├── reports
│   │   │       │   ├── cts
│   │   │       │   ├── cvc
│   │   │       │   ├── floorplan
│   │   │       │   ├── klayout
│   │   │       │   ├── lvs
│   │   │       │   ├── magic
│   │   │       │   ├── placement
│   │   │       │   ├── routing
│   │   │       │   └── synthesis
│   │   │       │       ├── 1-yosys_4.chk.rpt
│   │   │       │       ├── 1-yosys_4.stat.rpt
│   │   │       │       ├── 1-yosys_dff.stat
│   │   │       │       ├── 1-yosys_pre.stat
│   │   │       │       ├── 2-opensta.min_max.rpt
│   │   │       │       ├── 2-opensta.rpt
│   │   │       │       ├── 2-opensta.slew.rpt
│   │   │       │       ├── 2-opensta.timing.rpt
│   │   │       │       ├── 2-opensta_tns.rpt
│   │   │       │       └── 2-opensta_wns.rpt
│   │   │       ├── results
│   │   │       │   ├── cts
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── cvc
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── floorplan
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── klayout
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── lvs
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── magic
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── placement
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   ├── routing
│   │   │       │   │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │   └── synthesis
│   │   │       │       ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │       │       └── picorv32a.synthesis.v
│   │   │       └── tmp
│   │   │           ├── cts
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── cvc
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── floorplan
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── klayout
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── lvs
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── magic
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── merged.lef
│   │   │           ├── merged_unpadded.lef
│   │   │           ├── met_layers_list.txt
│   │   │           ├── placement
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── routing
│   │   │           │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           ├── sky130_fd_sc_hd__tt_025C_1v80.no_pg.lib
│   │   │           ├── synthesis
│   │   │           │   ├── hierarchy.dot
│   │   │           │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │           │   └── yosys.sdc
│   │   │           ├── tracks_copy.info
│   │   │           ├── trimmed.lib
│   │   │           └── trimmed.lib.exclude.list
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── picorv32a.sdc
│   │       └── picorv32a.v
│   ├── point_add
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── ecg.v
│   │       └── point_add.sdc
│   ├── point_scalar_mult
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── ecg.v
│   │       └── point_scalar_mult.sdc
│   ├── PPU
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── PPU.v
│   ├── README.md
│   ├── s44
│   │   ├── config.tcl
│   │   ├── pdn.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── lut_s44.v
│   │       └── lut.v
│   ├── salsa20
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── salsa20.sdc
│   │       └── salsa20.v
│   ├── sha3
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── sha3.sdc
│   │       └── sha3.v
│   ├── sha512
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── sha512.sdc
│   │       └── sha512.v
│   ├── sound
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── dsp_dma_identification_rom.hex
│   │       ├── opl2_attack_rom.hex
│   │       ├── opl2_waveform_rom.hex
│   │       └── sound.v
│   ├── spm
│   │   ├── config.json
│   │   ├── config.tcl
│   │   ├── pin_order.cfg
│   │   ├── runs
│   │   │   ├── 19-05_19-02
│   │   │   │   ├── cmds.log
│   │   │   │   ├── config.tcl
│   │   │   │   ├── logs
│   │   │   │   │   ├── 0-prep_runtime.txt
│   │   │   │   │   ├── 14-write_verilog.log
│   │   │   │   │   ├── 14-write_verilog_runtime.txt
│   │   │   │   │   ├── 16-write_verilog.log
│   │   │   │   │   ├── 16-write_verilog_runtime.txt
│   │   │   │   │   ├── 20-write_verilog.log
│   │   │   │   │   ├── 20-write_verilog_runtime.txt
│   │   │   │   │   ├── 26-write_verilog.log
│   │   │   │   │   ├── 26-write_verilog_runtime.txt
│   │   │   │   │   ├── 9-write_verilog.log
│   │   │   │   │   ├── 9-write_verilog_runtime.txt
│   │   │   │   │   ├── cts
│   │   │   │   │   │   ├── 13-cts.log
│   │   │   │   │   │   └── 13-cts_runtime.txt
│   │   │   │   │   ├── cvc
│   │   │   │   │   │   ├── 42-cvc_runtime.txt
│   │   │   │   │   │   └── 42-cvc_screen.log
│   │   │   │   │   ├── floorplan
│   │   │   │   │   │   ├── 3-verilog2def.openroad.log
│   │   │   │   │   │   ├── 3-verilog2def_openroad_runtime.txt
│   │   │   │   │   │   ├── 4-ioPlacer.log
│   │   │   │   │   │   ├── 4-ioPlacer_runtime.txt
│   │   │   │   │   │   ├── 5-tapcell.log
│   │   │   │   │   │   ├── 5-tapcell_runtime.txt
│   │   │   │   │   │   ├── 7-pdn.log
│   │   │   │   │   │   └── 7-pdn_runtime.txt
│   │   │   │   │   ├── flow_summary.log
│   │   │   │   │   ├── klayout
│   │   │   │   │   │   ├── 12-klayout.scrot.log
│   │   │   │   │   │   ├── 12-klayout_scrot_runtime.txt
│   │   │   │   │   │   ├── 15-klayout.scrot.log
│   │   │   │   │   │   ├── 15-klayout_scrot_runtime.txt
│   │   │   │   │   │   ├── 22-klayout.scrot.log
│   │   │   │   │   │   ├── 22-klayout_scrot_runtime.txt
│   │   │   │   │   │   ├── 28-klayout.scrot.log
│   │   │   │   │   │   ├── 28-klayout_scrot_runtime.txt
│   │   │   │   │   │   ├── 32-klayout.log
│   │   │   │   │   │   ├── 32-klayout_runtime.txt
│   │   │   │   │   │   ├── 33-klayout.scrot.log
│   │   │   │   │   │   ├── 33-klayout_scrot_runtime.txt
│   │   │   │   │   │   ├── 34-klayout.xor.log
│   │   │   │   │   │   ├── 35-klayout.scrot.log
│   │   │   │   │   │   ├── 35-klayout_scrot_runtime.txt
│   │   │   │   │   │   ├── 36-klayout.xor.log
│   │   │   │   │   │   ├── 36-klayout_xor_runtime.txt
│   │   │   │   │   │   ├── 6-klayout.scrot.log
│   │   │   │   │   │   └── 6-klayout_scrot_runtime.txt
│   │   │   │   │   ├── lvs
│   │   │   │   │   │   ├── 25-write_powered_verilog.log
│   │   │   │   │   │   ├── 38-lvs.lef.log
│   │   │   │   │   │   └── 38-lvs_runtime.txt
│   │   │   │   │   ├── magic
│   │   │   │   │   │   ├── 27-magic.log
│   │   │   │   │   │   ├── 29-magic.mag.gds_ptrs.log
│   │   │   │   │   │   ├── 30-magic.lef.log
│   │   │   │   │   │   ├── 31-magic_gen_runtime.txt
│   │   │   │   │   │   ├── 31-magic.maglef.log
│   │   │   │   │   │   ├── 37-magic_ext2spice.feedback.txt
│   │   │   │   │   │   ├── 37-magic_ext_spice_runtime.txt
│   │   │   │   │   │   ├── 37-magic_spice.log
│   │   │   │   │   │   ├── 39-magic.drc.log
│   │   │   │   │   │   └── 39-magic_drc_runtime.txt
│   │   │   │   │   ├── placement
│   │   │   │   │   │   ├── 11-opendp.log
│   │   │   │   │   │   ├── 11-opendp_runtime.txt
│   │   │   │   │   │   ├── 15-resizer_timing.log
│   │   │   │   │   │   ├── 15-resizer_timing_runtime.txt
│   │   │   │   │   │   ├── 8-replace.log
│   │   │   │   │   │   ├── 8-replace_runtime.txt
│   │   │   │   │   │   ├── 8-resizer.log
│   │   │   │   │   │   └── 8-resizer_runtime.txt
│   │   │   │   │   ├── routing
│   │   │   │   │   │   ├── 18-fastroute.log
│   │   │   │   │   │   ├── 18-fastroute_runtime.txt
│   │   │   │   │   │   ├── 19-addspacers.log
│   │   │   │   │   │   ├── 19-addspacers_runtime.txt
│   │   │   │   │   │   ├── 21-tritonRoute.log
│   │   │   │   │   │   ├── 21-tritonRoute_runtime.txt
│   │   │   │   │   │   ├── 23-spef_extraction.log
│   │   │   │   │   │   ├── 23-spef_extraction_runtime.txt
│   │   │   │   │   │   ├── 40-or_antenna.log
│   │   │   │   │   │   ├── 41-or_antenna_runtime.txt
│   │   │   │   │   │   └── fastroute.log
│   │   │   │   │   └── synthesis
│   │   │   │   │       ├── 10-opensta_post_resizer
│   │   │   │   │       ├── 10-opensta_post_resizer_runtime.txt
│   │   │   │   │       ├── 17-opensta_post_resizer_timing
│   │   │   │   │       ├── 17-opensta_post_resizer_timing_runtime.txt
│   │   │   │   │       ├── 1-yosys.log
│   │   │   │   │       ├── 1-yosys_runtime.txt
│   │   │   │   │       ├── 24-opensta_spef
│   │   │   │   │       ├── 24-opensta_spef_runtime.txt
│   │   │   │   │       ├── 2-opensta
│   │   │   │   │       └── 2-opensta_runtime.txt
│   │   │   │   ├── OPENLANE_VERSION
│   │   │   │   ├── PDK_SOURCES
│   │   │   │   ├── reports
│   │   │   │   │   ├── cts
│   │   │   │   │   │   ├── 13-cts_clock_skew.rpt
│   │   │   │   │   │   ├── 13-cts.min_max.rpt
│   │   │   │   │   │   ├── 13-cts.rpt
│   │   │   │   │   │   ├── 13-cts.timing.rpt
│   │   │   │   │   │   ├── 13-cts_tns.rpt
│   │   │   │   │   │   └── 13-cts_wns.rpt
│   │   │   │   │   ├── cvc
│   │   │   │   │   ├── final_summary_report.csv
│   │   │   │   │   ├── floorplan
│   │   │   │   │   │   ├── 3-verilog2def.core_area.rpt
│   │   │   │   │   │   └── 3-verilog2def.die_area.rpt
│   │   │   │   │   ├── klayout
│   │   │   │   │   │   ├── 34-klayout.xor.rpt
│   │   │   │   │   │   └── 36-klayout.xor.rpt
│   │   │   │   │   ├── lvs
│   │   │   │   │   ├── magic
│   │   │   │   │   │   ├── 39-magic.drc
│   │   │   │   │   │   ├── 39-magic.drc.klayout.xml
│   │   │   │   │   │   ├── 39-magic.drc.rdb
│   │   │   │   │   │   ├── 39-magic.drc.tcl
│   │   │   │   │   │   └── 39-magic.tr.drc
│   │   │   │   │   ├── manufacturability_report.rpt
│   │   │   │   │   ├── placement
│   │   │   │   │   │   ├── 8-replace.min_max.rpt
│   │   │   │   │   │   ├── 8-replace.rpt
│   │   │   │   │   │   ├── 8-replace.timing.rpt
│   │   │   │   │   │   ├── 8-replace_tns.rpt
│   │   │   │   │   │   └── 8-replace_wns.rpt
│   │   │   │   │   ├── routed_runtime.txt
│   │   │   │   │   ├── routing
│   │   │   │   │   │   ├── 18-fastroute.min_max.rpt
│   │   │   │   │   │   ├── 18-fastroute.rpt
│   │   │   │   │   │   ├── 18-fastroute.timing.rpt
│   │   │   │   │   │   ├── 18-fastroute_tns.rpt
│   │   │   │   │   │   ├── 18-fastroute_wns.rpt
│   │   │   │   │   │   ├── 21-tritonRoute.drc
│   │   │   │   │   │   ├── 21-tritonRoute.klayout.xml
│   │   │   │   │   │   └── 41-antenna.rpt
│   │   │   │   │   ├── runtime_summary_report.rpt
│   │   │   │   │   ├── runtime_summary_report.rpt.parsable
│   │   │   │   │   ├── synthesis
│   │   │   │   │   │   ├── 10-opensta_post_resizer.min_max.rpt
│   │   │   │   │   │   ├── 10-opensta_post_resizer.rpt
│   │   │   │   │   │   ├── 10-opensta_post_resizer.slew.rpt
│   │   │   │   │   │   ├── 10-opensta_post_resizer.timing.rpt
│   │   │   │   │   │   ├── 10-opensta_post_resizer_tns.rpt
│   │   │   │   │   │   ├── 10-opensta_post_resizer_wns.rpt
│   │   │   │   │   │   ├── 17-opensta_post_resizer_timing.min_max.rpt
│   │   │   │   │   │   ├── 17-opensta_post_resizer_timing.rpt
│   │   │   │   │   │   ├── 17-opensta_post_resizer_timing.slew.rpt
│   │   │   │   │   │   ├── 17-opensta_post_resizer_timing.timing.rpt
│   │   │   │   │   │   ├── 17-opensta_post_resizer_timing_tns.rpt
│   │   │   │   │   │   ├── 17-opensta_post_resizer_timing_wns.rpt
│   │   │   │   │   │   ├── 1-yosys_4.chk.rpt
│   │   │   │   │   │   ├── 1-yosys_4.stat.rpt
│   │   │   │   │   │   ├── 1-yosys_dff.stat
│   │   │   │   │   │   ├── 1-yosys_pre.stat
│   │   │   │   │   │   ├── 24-opensta_spef.min_max.rpt
│   │   │   │   │   │   ├── 24-opensta_spef.rpt
│   │   │   │   │   │   ├── 24-opensta_spef.slew.rpt
│   │   │   │   │   │   ├── 24-opensta_spef.timing.rpt
│   │   │   │   │   │   ├── 24-opensta_spef_tns.rpt
│   │   │   │   │   │   ├── 24-opensta_spef_wns.rpt
│   │   │   │   │   │   ├── 2-opensta.min_max.rpt
│   │   │   │   │   │   ├── 2-opensta.rpt
│   │   │   │   │   │   ├── 2-opensta.slew.rpt
│   │   │   │   │   │   ├── 2-opensta.timing.rpt
│   │   │   │   │   │   ├── 2-opensta_tns.rpt
│   │   │   │   │   │   └── 2-opensta_wns.rpt
│   │   │   │   │   └── total_runtime.txt
│   │   │   │   ├── results
│   │   │   │   │   ├── cts
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.cts.def
│   │   │   │   │   │   └── spm.cts.def.png
│   │   │   │   │   ├── cvc
│   │   │   │   │   │   ├── cvc_spm.debug.gz
│   │   │   │   │   │   ├── cvc_spm.error.gz
│   │   │   │   │   │   ├── cvc_spm.log
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.cdl
│   │   │   │   │   │   └── spm.power
│   │   │   │   │   ├── floorplan
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.floorplan.def
│   │   │   │   │   │   └── spm.floorplan.def.png
│   │   │   │   │   ├── klayout
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.gds
│   │   │   │   │   │   ├── spm.gds.png
│   │   │   │   │   │   ├── spm.lyp
│   │   │   │   │   │   ├── spm.xor.gds
│   │   │   │   │   │   ├── spm.xor.gds.png
│   │   │   │   │   │   └── spm.xor.xml
│   │   │   │   │   ├── lvs
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.lvs.lef.json
│   │   │   │   │   │   ├── spm.lvs.lef.log
│   │   │   │   │   │   ├── spm.lvs_parsed.lef.log
│   │   │   │   │   │   └── spm.lvs.powered.v
│   │   │   │   │   ├── magic
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.drc.mag
│   │   │   │   │   │   ├── spm.gds
│   │   │   │   │   │   ├── spm.gds.png
│   │   │   │   │   │   ├── spm.lef
│   │   │   │   │   │   ├── spm.lef.mag
│   │   │   │   │   │   ├── spm.lef.spice
│   │   │   │   │   │   ├── spm.mag
│   │   │   │   │   │   └── spm.spice
│   │   │   │   │   ├── placement
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.placement.def
│   │   │   │   │   │   └── spm.placement.def.png
│   │   │   │   │   ├── routing
│   │   │   │   │   │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │   │   ├── spm.def
│   │   │   │   │   │   ├── spm.def.png
│   │   │   │   │   │   ├── spm.def.ref
│   │   │   │   │   │   └── spm.spef
│   │   │   │   │   └── synthesis
│   │   │   │   │       ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │   │       ├── spm.synthesis_cts.v
│   │   │   │   │       ├── spm.synthesis_optimized.v
│   │   │   │   │       ├── spm.synthesis_preroute.v
│   │   │   │   │       └── spm.synthesis.v
│   │   │   │   └── tmp
│   │   │   │       ├── cts
│   │   │   │       │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       ├── cts.lib
│   │   │   │       ├── cts.lib.exclude.list
│   │   │   │       ├── cvc
│   │   │   │       │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       ├── floorplan
│   │   │   │       │   ├── 3-verilog2def_openroad.def
│   │   │   │       │   ├── 4-ioPlacer.def
│   │   │   │       │   ├── 7-pdn.def
│   │   │   │       │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       ├── klayout
│   │   │   │       │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       ├── lvs
│   │   │   │       │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       │   └── setup_file.lef.lvs
│   │   │   │       ├── magic
│   │   │   │       │   ├── magic_gds_ptrs.mag
│   │   │   │       │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       │   ├── sky130_fd_sc_hd__a21oi_2.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__a22o_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__a31oi_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__and2_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__buf_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__clkbuf_16.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__clkbuf_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__clkbuf_2.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__decap_12.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__decap_3.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__decap_4.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__decap_6.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__decap_8.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__dfrtp_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__dlymetal6s2s_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__fill_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__fill_2.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__inv_2.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__o2bb2a_1.ext
│   │   │   │       │   ├── sky130_fd_sc_hd__tapvpwrvgnd_1.ext
│   │   │   │       │   └── spm.ext
│   │   │   │       ├── magic_spice.tcl
│   │   │   │       ├── merged.lef
│   │   │   │       ├── merged_unpadded.lef
│   │   │   │       ├── met_layers_list.txt
│   │   │   │       ├── placement
│   │   │   │       │   ├── 15-resizer_timing.def
│   │   │   │       │   ├── 8-replace.def
│   │   │   │       │   ├── 8-resizer.def
│   │   │   │       │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       ├── resizer.lib
│   │   │   │       ├── resizer.lib.exclude.list
│   │   │   │       ├── routing
│   │   │   │       │   ├── 18-fastroute.def
│   │   │   │       │   ├── 18-fastroute.guide
│   │   │   │       │   ├── 19-addspacers.def
│   │   │   │       │   ├── 21-tritonRoute.guide
│   │   │   │       │   ├── 21-tritonRoute.param
│   │   │   │       │   ├── 21-tritonRoute_TA.def
│   │   │   │       │   ├── 25-spm.powered.def
│   │   │   │       │   └── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       ├── sky130_fd_sc_hd__tt_025C_1v80.no_pg.lib
│   │   │   │       ├── synthesis
│   │   │   │       │   ├── hierarchy.dot
│   │   │   │       │   ├── merged_unpadded.lef -> ../../tmp/merged_unpadded.lef
│   │   │   │       │   └── yosys.sdc
│   │   │   │       ├── tracks_copy.info
│   │   │   │       ├── trimmed.lib
│   │   │   │       └── trimmed.lib.exclude.list
│   │   │   └── 29-06_07-34
│   │   │       ├── cmds.log
│   │   │       ├── config.tcl
│   │   │       ├── logs
│   │   │       │   ├── 0-prep_runtime.txt
│   │   │       │   ├── cts
│   │   │       │   ├── cvc
│   │   │       │   ├── floorplan
│   │   │       │   │   ├── 3-verilog2def.openroad.log
│   │   │       │   │   ├── 3-verilog2def_openroad_runtime.txt
│   │   │       │   │   ├── 4-ioPlacer.log
│   │   │       │   │   ├── 4-ioPlacer_runtime.txt
│   │   │       │   │   ├── 5-tapcell.log
│   │   │       │   │   ├── 5-tapcell_runtime.txt
│   │   │       │   │   ├── 7-pdn.log
│   │   │       │   │   └── 7-pdn_runtime.txt
│   │   │       │   ├── flow_summary.log
│   │   │       │   ├── klayout
│   │   │       │   │   ├── 6-klayout.scrot.log
│   │   │       │   │   └── 6-klayout_scrot_runtime.txt
│   │   │       │   ├── lvs
│   │   │       │   ├── magic
│   │   │       │   ├── placement
│   │   │       │   ├── routing
│   │   │       │   └── synthesis
│   │   │       │       ├── 1-yosys.log
│   │   │       │       ├── 1-yosys_runtime.txt
│   │   │       │       ├── 2-opensta
│   │   │       │       └── 2-opensta_runtime.txt
│   │   │       ├── OPENLANE_VERSION
│   │   │       ├── PDK_SOURCES
│   │   │       ├── reports
│   │   │       │   ├── cts
│   │   │       │   ├── cvc
│   │   │       │   ├── floorplan
│   │   │       │   │   ├── 3-verilog2def.core_area.rpt
│   │   │       │   │   └── 3-verilog2def.die_area.rpt
│   │   │       │   ├── klayout
│   │   │       │   ├── lvs
│   │   │       │   ├── magic
│   │   │       │   ├── placement
│   │   │       │   ├── routing
│   │   │       │   └── synthesis
│   │   │       │       ├── 1-yosys_4.chk.rpt
│   │   │       │       ├── 1-yosys_4.stat.rpt
│   │   │       │       ├── 1-yosys_dff.stat
│   │   │       │       ├── 1-yosys_pre.stat
│   │   │       │       ├── 2-opensta.min_max.rpt
│   │   │       │       ├── 2-opensta.rpt
│   │   │       │       ├── 2-opensta.slew.rpt
│   │   │       │       ├── 2-opensta.timing.rpt
│   │   │       │       ├── 2-opensta_tns.rpt
│   │   │       │       └── 2-opensta_wns.rpt
│   │   │       ├── results
│   │   │       │   ├── cts
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   ├── cvc
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   ├── floorplan
│   │   │       │   │   ├── merged_unpadded.lef
│   │   │       │   │   ├── spm.floorplan.def
│   │   │       │   │   └── spm.floorplan.def.png
│   │   │       │   ├── klayout
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   ├── lvs
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   ├── magic
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   ├── placement
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   ├── routing
│   │   │       │   │   └── merged_unpadded.lef
│   │   │       │   └── synthesis
│   │   │       │       ├── merged_unpadded.lef
│   │   │       │       └── spm.synthesis.v
│   │   │       └── tmp
│   │   │           ├── cts
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── cvc
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── floorplan
│   │   │           │   ├── 3-verilog2def_openroad.def
│   │   │           │   ├── 4-ioPlacer.def
│   │   │           │   ├── 7-pdn.def
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── klayout
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── lvs
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── magic
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── merged.lef
│   │   │           ├── merged_unpadded.lef
│   │   │           ├── met_layers_list.txt
│   │   │           ├── placement
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── routing
│   │   │           │   └── merged_unpadded.lef
│   │   │           ├── sky130_fd_sc_hd__tt_025C_1v80.no_pg.lib
│   │   │           ├── synthesis
│   │   │           │   ├── hierarchy.dot
│   │   │           │   ├── merged_unpadded.lef
│   │   │           │   └── yosys.sdc
│   │   │           ├── tracks_copy.info
│   │   │           ├── trimmed.lib
│   │   │           └── trimmed.lib.exclude.list
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── spm.sdc
│   │       └── spm.v
│   ├── synth_ram
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── synth_ram.v
│   ├── usb
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── usb2p0_core.v
│   ├── usb_cdc_core
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── usb_cdc_core.sdc
│   │       ├── usb_cdc_core.v
│   │       ├── usb_desc_rom.v
│   │       ├── usbf_crc16.v
│   │       ├── usbf_defs.v
│   │       ├── usbf_device_core.v
│   │       ├── usbf_sie_rx.v
│   │       └── usbf_sie_tx.v
│   ├── usbf_device
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       └── usbf_device.v
│   ├── wbqspiflash
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── wbqspiflash.sdc
│   │       └── wbqspiflash.v
│   ├── xtea
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── xtea.sdc
│   │       └── xtea.v
│   ├── y_dct
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── y_dct.sdc
│   │       └── y_dct.v
│   ├── y_huff
│   │   ├── config.tcl
│   │   ├── sky130A_sky130_fd_sc_hd_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hdll_config.tcl
│   │   ├── sky130A_sky130_fd_sc_hs_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ls_config.tcl
│   │   ├── sky130A_sky130_fd_sc_ms_config.tcl
│   │   └── src
│   │       ├── y_huff.sdc
│   │       └── y_huff.v
│   └── zipdiv
│       ├── config.tcl
│       ├── sky130A_sky130_fd_sc_hd_config.tcl
│       ├── sky130A_sky130_fd_sc_hdll_config.tcl
│       ├── sky130A_sky130_fd_sc_hs_config.tcl
│       ├── sky130A_sky130_fd_sc_ls_config.tcl
│       ├── sky130A_sky130_fd_sc_ms_config.tcl
│       └── src
│           ├── zipdiv.sdc
│           └── zipdiv.v
├── docker_build
│   ├── docker
│   │   ├── antmicro_yosys
│   │   │   └── Dockerfile
│   │   ├── cugr
│   │   │   └── Dockerfile
│   │   ├── cvc
│   │   │   ├── cvc-1.0.0.tar.gz
│   │   │   └── Dockerfile
│   │   ├── drcu
│   │   │   └── Dockerfile
│   │   ├── klayout
│   │   │   └── Dockerfile
│   │   ├── magic
│   │   │   └── Dockerfile
│   │   ├── netgen
│   │   │   └── Dockerfile
│   │   ├── opendp
│   │   │   └── Dockerfile
│   │   ├── openphysyn
│   │   │   └── Dockerfile
│   │   ├── openroad_app
│   │   │   ├── Dockerfile
│   │   │   ├── ignore_obs_outside.patch
│   │   │   ├── opendp-diamond-search.patch
│   │   │   ├── pdn_gen_core_ring_fix.patch
│   │   │   ├── pdngen_export_subst.patch
│   │   │   ├── rails.patch
│   │   │   └── setup_local.patch
│   │   ├── opensta
│   │   │   └── Dockerfile
│   │   ├── padring
│   │   │   └── Dockerfile
│   │   ├── replace
│   │   │   └── Dockerfile
│   │   ├── route
│   │   │   └── Dockerfile
│   │   ├── vlogtoverilog
│   │   │   └── Dockerfile
│   │   └── yosys
│   │       └── Dockerfile
│   ├── Dockerfile
│   ├── hooks
│   │   └── build
│   ├── Makefile
│   ├── README.md
│   └── tar
│       ├── antmicro_yosys.tar.gz
│       ├── cugr.tar.gz
│       ├── cvc.tar.gz
│       ├── drcu.tar.gz
│       ├── klayout.tar.gz
│       ├── magic.tar.gz
│       ├── netgen.tar.gz
│       ├── opendp.tar.gz
│       ├── openphysyn.tar.gz
│       ├── openroad_app.tar.gz
│       ├── opensta.tar.gz
│       ├── padring.tar.gz
│       ├── replace.tar.gz
│       ├── route.tar.gz
│       ├── vlogtoverilog.tar.gz
│       └── yosys.tar.gz
├── docs
│   ├── environment.yml
│   ├── _ext
│   │   ├── image_links.py
│   │   ├── markdown_code_links.py
│   │   ├── markdown_cross_doc_section_links.py
│   │   └── toc_from_markdown.py
│   ├── Makefile
│   ├── requirements.txt
│   ├── source
│   │   ├── advanced_power_grid_control.md
│   │   ├── advanced_readme.md
│   │   ├── chip_integration.md
│   │   ├── hardening_macros.md
│   │   ├── Manual_PDK_installation.md
│   │   ├── OpenLANE_commands.md
│   │   └── PDK_STRUCTURE.md
│   └── _static
│       ├── openlane.flow.1.png
│       └── striVe.jpeg
├── flow.tcl
├── LICENSE
├── Makefile
├── README.md
├── regression_results
│   ├── benchmark_results
│   │   ├── SW_HD.csv
│   │   ├── SW_HD.html
│   │   ├── SW_HDLL.csv
│   │   ├── SW_HDLL.html
│   │   ├── SW_HS.csv
│   │   ├── SW_HS.html
│   │   ├── SW_LS.csv
│   │   ├── SW_LS.html
│   │   ├── SW_MS.csv
│   │   └── SW_MS.html
│   ├── columns_defintions.md
│   └── README.md
├── report_generation_wrapper.py
├── run_designs.py
└── scripts
    ├── add_def_obstructions.py
    ├── append_special_nets.py
    ├── apply_def_template.py
    ├── base.sdc
    ├── cleanupConfigs.py
    ├── compare_regression_design.py
    ├── compare_regression_reports.py
    ├── config
    │   ├── config_get.sh
    │   ├── config.py
    │   ├── generate_config.py
    │   ├── generate_config.sh
    │   ├── __pycache__
    │   │   └── config.cpython-36.pyc
    │   └── regression.config
    ├── consoletext.py
    ├── contextualize.py
    ├── count_lvs.py
    ├── csv2html
    │   ├── csv2html.py
    │   ├── static
    │   │   └── style.css
    │   └── templates
    │       ├── main.html
    │       └── _partial.html
    ├── cts
    │   └── cts_simple.pl
    ├── cvc
    │   └── sky130A
    │       ├── cvcrc.sky130A
    │       └── cvc.sky130A.models
    ├── expand_diearea.sh
    ├── extract_antenna_violators.py
    ├── extract_coreinfo.sh
    ├── extract_metal_layers.py
    ├── fakeDiodeReplace.py
    ├── fixlayernames.sh
    ├── gds2lef.py
    ├── get_core_dimensions.py
    ├── grepCount.sh
    ├── io_place.py
    ├── klayout
    │   ├── def2gds.py
    │   ├── def2gds.sh
    │   ├── mv_shapes.py
    │   ├── mv_shapes.sh
    │   ├── run_drc.sh
    │   ├── scrotLayout.py
    │   ├── scrotLayout.sh
    │   ├── xor.drc
    │   └── xor.sh
    ├── label_macro_pins.py
    ├── label_padframe.py
    ├── lef_copy_annotation.py
    ├── lef_enforce_manufacturing_grid.py
    ├── li1_hack_end.py
    ├── li1_hack_start.py
    ├── libtrim.pl
    ├── logic_equiv_check.tcl
    ├── magic
    │   ├── drc_batch.tcl
    │   ├── drc.tcl
    │   ├── erase_box.sh
    │   ├── gdses2mags.tcl
    │   ├── gds_pointers.tcl
    │   ├── lefs2maglefs.tcl
    │   ├── lef.tcl
    │   ├── mag_gds.tcl
    │   ├── maglef.tcl
    │   └── mag.tcl
    ├── magic_drc_to_rdb.py
    ├── magic_drc_to_tcl.py
    ├── magic_drc_to_tr_drc.py
    ├── manual_macro_place.py
    ├── mark_component_fixed.sh
    ├── merge_components.sh
    ├── mergeLef.py
    ├── mv_components.sh
    ├── mv_pins.sh
    ├── obs_above.py
    ├── obs.py
    ├── openPhySyn.tcl
    ├── openroad
    │   ├── or_antenna_check.tcl
    │   ├── or_basic_mp.tcl
    │   ├── or_cts.tcl
    │   ├── or_diodes.tcl
    │   ├── or_droute.tcl
    │   ├── or_fill.tcl
    │   ├── or_floorplan.tcl
    │   ├── or_groute.tcl
    │   ├── or_ioplacer.tcl
    │   ├── or_opendp.tcl
    │   ├── or_pdn.tcl
    │   ├── or_replace.tcl
    │   ├── or_resizer.tcl
    │   ├── or_resizer_timing.tcl
    │   ├── or_tapcell.tcl
    │   └── or_write_verilog.tcl
    ├── padframe2fp.py
    ├── padframe_extract_area.sh
    ├── padLefMacro.py
    ├── padringer.py
    ├── parse_klayout_xor_log.py
    ├── pfg.py
    ├── place_diodes.py
    ├── power_route.py
    ├── random_place.py
    ├── rectify_above.py
    ├── rectify.py
    ├── remove_components.sh
    ├── remove_def_component.sh
    ├── remove_empty_nets.sh
    ├── remove_empty_pins.py
    ├── remove_empty_ports.py
    ├── removeEnvVar.sh
    ├── remove_nets.sh
    ├── remove_pins.sh
    ├── replace_gp.tcl
    ├── replace_prefix_from_def_instances.py
    ├── replicateDesignsConfigs.py
    ├── report
    │   ├── get_best.py
    │   ├── get_file_name.py
    │   ├── __pycache__
    │   │   ├── get_file_name.cpython-36.pyc
    │   │   └── report.cpython-36.pyc
    │   ├── report.py
    │   └── report.sh
    ├── setLayerTracks.py
    ├── spef_extractor
    │   ├── lef_def_parser
    │   │   ├── def_parser.py
    │   │   ├── def_util.py
    │   │   ├── __init__.py
    │   │   ├── lef_parser.py
    │   │   ├── lef_util.py
    │   │   ├── LICENSE
    │   │   ├── __pycache__
    │   │   │   ├── def_parser.cpython-36.pyc
    │   │   │   ├── def_util.cpython-36.pyc
    │   │   │   ├── __init__.cpython-36.pyc
    │   │   │   ├── lef_parser.cpython-36.pyc
    │   │   │   ├── lef_util.cpython-36.pyc
    │   │   │   └── util.cpython-36.pyc
    │   │   └── util.py
    │   ├── LICENSE
    │   ├── main.py
    │   └── README.md
    ├── sta.tcl
    ├── synth_exp
    │   ├── analyze.pl
    │   ├── table.css
    │   └── utils.js
    ├── synth.tcl
    ├── synth_top.tcl
    ├── tcl_commands
    │   ├── all.tcl
    │   ├── checkers.tcl
    │   ├── cts.tcl
    │   ├── cvc.tcl
    │   ├── floorplan.tcl
    │   ├── init_design.tcl
    │   ├── klayout.tcl
    │   ├── list.txt
    │   ├── lvs.tcl
    │   ├── magic.tcl
    │   ├── pkgIndex.tcl
    │   ├── placement.tcl
    │   ├── README.md
    │   ├── refresh.tcl
    │   ├── routing.tcl
    │   └── synthesis.tcl
    ├── tksimpledialog.py
    ├── topModuleGen
    │   ├── README.md
    │   └── src
    │       ├── padHelper.py
    │       └── TopModuleGen.py
    ├── tr2klayout.py
    ├── tritonRoute.param
    ├── unroller.sh
    ├── updateDesignsConfigs.py
    ├── utils
    │   ├── deflef_utils.tcl
    │   ├── fake_display_buffer.tcl
    │   ├── __init__.py
    │   ├── pkgIndex.tcl
    │   ├── __pycache__
    │   │   ├── __init__.cpython-36.pyc
    │   │   └── utils.cpython-36.pyc
    │   ├── utils.py
    │   └── utils.tcl
    ├── widenSiteLef.py
    ├── wrap_lef_macro.py
    ├── write_powered_def.py
    ├── yosys_rewrite_verilog.tcl
    ├── zeroize_origin_def.py
    └── zeroize_origin_lef.py

263 directories, 1009 files


</details>


- The Open Lane Directory has the following folders
<p align="center">
  <img width="600" height="100" src="../images/13.png">
</p>
- we will be working in the openlane directory and PDKs directory as the name suggests contains all the PDK files
<p align="center">
  <img width="800" height="350" src="../images/14.png">
</p>

- these folders are in sky130A directory: (a) `libs.ref` and (b) `libs.tech`
	- libs.ref contains all the process or technology specific files
	- In this workshop, we are working on the **`sky130_fd_sc_hd`** files which states for **`Sky130 foundry std. cell. high definition `**


##### Design Preparation

- OpenLane can be invoked using docker command using the interactive session.

<p align="center">
  <img width="800" height="350" src="../images/15.png">
</p>

- As shown in image `./flow.tcl -interactive` runs the openlane in interactive mode.
- And `package require openlane 0.9` has to be run

OpenLane has multiple design files and we are  working on `picorv32a design`

<p align="center">
  <img width="850" height="150" src="../images/16.png">
</p>

- Next We will setup the design stage for the flow and to begin with synthesis of a design:
  `prep -design picorv32a`
<p align="center">
  <img width="1000" height="400" src="../images/17.png">
</p>

- This creates the new directory named `runs` under picorv32a folder that consists of folder with name as datetime when the above command is run. It consists of results, reports, command logs, etc. as shown below.

<p align="center">
  <img width="1000" height="400" src="../images/18.png">
</p>

Run synthesis with the below command:
`run_synthesis`

- After the synthesis step is complete, reports and results are generated.

Output stats after the synthesis are as follows:
```shell
28.  Printing statistics.

=== picorv32a ===

   Number of wires:              14596
   Number of wire bits:          14978
   Number of public wires:        1565
   Number of public wire bits:    1947
   Number of memories:               0
   Number of memory bits:            0
   Number of processes:              0
   Number of cells:              14876
     sky130_fd_sc_hd__a2111o_2       1
     sky130_fd_sc_hd__a211o_2       35
     sky130_fd_sc_hd__a211oi_2      60
     sky130_fd_sc_hd__a21bo_2      149
     sky130_fd_sc_hd__a21boi_2       8
     sky130_fd_sc_hd__a21o_2        57
     sky130_fd_sc_hd__a21oi_2      244
     sky130_fd_sc_hd__a221o_2       86
     sky130_fd_sc_hd__a22o_2      1013
     sky130_fd_sc_hd__a2bb2o_2    1748
     sky130_fd_sc_hd__a2bb2oi_2     81
     sky130_fd_sc_hd__a311o_2        2
     sky130_fd_sc_hd__a31o_2        49
     sky130_fd_sc_hd__a31oi_2        7
     sky130_fd_sc_hd__a32o_2        46
     sky130_fd_sc_hd__a41o_2         1
     sky130_fd_sc_hd__and2_2       157
     sky130_fd_sc_hd__and3_2        58
     sky130_fd_sc_hd__and4_2       345
     sky130_fd_sc_hd__and4b_2        1
     sky130_fd_sc_hd__buf_1       1656
     sky130_fd_sc_hd__buf_2          8
     sky130_fd_sc_hd__conb_1        42
     sky130_fd_sc_hd__dfxtp_2     1613
     sky130_fd_sc_hd__inv_2       1615
     sky130_fd_sc_hd__mux2_1      1224
     sky130_fd_sc_hd__mux2_2         2
     sky130_fd_sc_hd__mux4_1       221
     sky130_fd_sc_hd__nand2_2       78
     sky130_fd_sc_hd__nor2_2       524
     sky130_fd_sc_hd__nor2b_2        1
     sky130_fd_sc_hd__nor3_2        42
     sky130_fd_sc_hd__nor4_2         1
     sky130_fd_sc_hd__o2111a_2       2
     sky130_fd_sc_hd__o211a_2       69
     sky130_fd_sc_hd__o211ai_2       6
     sky130_fd_sc_hd__o21a_2        54
     sky130_fd_sc_hd__o21ai_2      141
     sky130_fd_sc_hd__o21ba_2      209
     sky130_fd_sc_hd__o21bai_2       1
     sky130_fd_sc_hd__o221a_2      204
     sky130_fd_sc_hd__o221ai_2       7
     sky130_fd_sc_hd__o22a_2      1312
     sky130_fd_sc_hd__o22ai_2       59
     sky130_fd_sc_hd__o2bb2a_2     119
     sky130_fd_sc_hd__o2bb2ai_2     92
     sky130_fd_sc_hd__o311a_2        8
     sky130_fd_sc_hd__o31a_2        19
     sky130_fd_sc_hd__o31ai_2        1
     sky130_fd_sc_hd__o32a_2       109
     sky130_fd_sc_hd__o41a_2         2
     sky130_fd_sc_hd__or2_2       1088
     sky130_fd_sc_hd__or2b_2        25
     sky130_fd_sc_hd__or3_2         68
     sky130_fd_sc_hd__or3b_2         5
     sky130_fd_sc_hd__or4_2         93
     sky130_fd_sc_hd__or4b_2         6
     sky130_fd_sc_hd__or4bb_2        2

   Chip area for module '\picorv32a': 147712.918400
 

```

Here the DFF count:  `sky130_fd_sc_hd__dfxtp_2` = `1613`

- And total number of cells = `14876`

    ```
  D flip-flop ratio 	= count of DFFs / total number of cells
  					= 1613 / 14876
  					= 0.108429685 (OR) 10.8429 %
    ``` 
