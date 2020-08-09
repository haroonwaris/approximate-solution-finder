****************************************************************************************************
      This code is provided here for educational purpose(s) only.  For questions/suggestions
 please email Haroon Waris (haroonwaris@nuaa.edu.cn) or Dr. Weiqiang Liu (liuweiqiang@nuaa.edu.cn)
****************************************************************************************************

This directory contains the Verilog sources of our paper, "AxRMs: Design and evaluation of approximate recursive multipliers under error constraint”, which is currently under review. 


1.  Exact_HA.v is the accurate half adder.
2.  Exact_FA.v is the accurate full adder.

3.  Exact_4x4.v is the exact 4x4 multiplier.
    Dependencies: Exact_FA.v, Exact_HA.v
	 
4.  ASF_4x4.v is the approximate 4x4 multiplier generated using proposed approximate solution finder (ASF).
    
5.  ASF_M8_1.v is the approximate 8x8 multiplier (Least approximated).
    Dependencies: ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

6.  ASF_M8_2.v is the approximate 8x8 multiplier (Two approximate 4x4 modules).
    Dependencies: ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

7.  ASF_M8_3.v is the approximate 8x8 multiplier (Three approximate 4x4 modules).
    Dependencies: ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

8.  ASF_M8_4.v is the approximate 8x8 multiplier (most approximated).
    Dependencies: ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

9.  ASF_M16_1.v is the approximate 16x16 multiplier (almost accurate multiplier).
    Dependencies: ASF_M8_1.v, ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

10. ASF_M16_2.v is the approximate 16x16 multiplier (Trade-off between hardware and efficiency).
    Dependencies: ASF_M8_2.v, ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

11. ASF_M16_3.v is the approximate 16x16 multiplier (Trade-off between hardware and efficiency).
    Dependencies: ASF_M8_3.v, ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v

12. ASF_M16_4.v is the approximate 16x16 multiplier (hardware-efficient multiplier).
    Dependencies: ASF_M8_4.v, ASF_4x4.v, Exact_4x4.v, Exact_FA.v, Exact_HA.v
