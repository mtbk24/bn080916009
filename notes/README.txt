bn080916009 GBMwLAT


grbm:  good fit, errors and stats.

sbpl:  good fit, errors and stats.  better stats than grbm.

copl:  bad.  doens't fit the high energy bgo, lat or lle data.  got errors without flags.  stats are large, meaning not a good fit.

grbm+lpow:  PL is a good slope and significance, but it only really contributes to the lower energies.  See Plots.  Had no problems getting 1-sigma errors.  2-sigma kept wanting to fit.  At 2-sigma, the uncertainty in the PL parameters became the problem.  No flags in the other params.  Better stats than grbm alone, but not better than sbpl alone.
   1    1   grbm       alpha               -0.742996    +/-  0.154397     
   2    1   grbm       beta                -2.17787     +/-  3.87567E-02  
   3    1   grbm       tem        keV      305.505      +/-  60.0652      
   4    1   grbm       norm                1.90143E-02  +/-  1.43343E-03  
   5    2   lpow       plIndex    NONE     -2.07713     +/-  0.535507     
   6    2   lpow       norm                9.92564E-04  +/-  1.50399E-03

sbpl+lpow:  Tried to get PL to stick at -1.8 or -1.9 so that the PL would contributed to the high-energy data, but it wouldn't stick.  It meandered back to -2.06.  At 1-sigma, got good errors.  At 2-sigma got flags on the PL params only.  AIC is better than sbpl alone, but BIC is worse, but not by much.
   1    1   sbpl       alpha      NONE     -0.907276    +/-  0.118440
   2    1   sbpl       beta       NONE     -2.18197     +/-  3.96240E-02  
   3    1   sbpl       ebreak     keV      215.640      +/-  16.6692      
   4    1   sbpl       norm                1.39326E-02  +/-  1.35470E-03  
   5    2   lpow       plIndex    NONE     -2.05816     +/-  0.498306     
   6    2   lpow       norm                8.95569E-04  +/-  1.32775E-03

copl+lpow:  The combination of PL and COPL at lower energies doesn't allow for a PL to stick at -2 to -2.3 slope.  Therefore, this combo doesn't match the high-energy data that dives downward, while this PL dives upward.  Fit looks good until about 1000 keV, then the PL dives upward with a slope of -1.8.  This fit doesn't fit the high-energy data.
   1    1   copl       cplIndex   NONE     -0.514566    +/-  7.92503E-02  
   2    1   copl       highEcut   NONE     259.416      +/-  26.0973      
   3    1   copl       norm                1.71153E-02  +/-  6.61318E-04  
   4    2   lpow       plIndex    NONE     -1.80533     +/-  1.00903E-02  
   5    2   lpow       norm                2.89971E-03  +/-  1.87707E-04

grbm+blackb:  Good params, fit, errors, and stats.  No bbody significant at lower energies.
   1    1   grbm       alpha               -1.22002     +/-  3.33989E-02  
   2    1   grbm       beta                -2.22958     +/-  2.39016E-02  
   3    1   grbm       tem        keV      1186.59      +/-  248.871      
   4    1   grbm       norm                1.25898E-02  +/-  7.00414E-04  
   5    2   blackb     kT         keV      42.6584      +/-  2.33410      
   6    2   blackb     norm                4.00278E-06  +/-  8.80072E-07

sbpl+blackb:
   1    1   sbpl       alpha      NONE     -1.26993     +/-  2.93023E-02  
   2    1   sbpl       beta       NONE     -2.22795     +/-  2.17042E-02  
   3    1   sbpl       ebreak     keV      523.497      +/-  96.7252      
   4    1   sbpl       norm                1.13664E-02  +/-  5.09215E-04  
   5    2   blackb     kT         keV      40.0156      +/-  2.16064      
   6    2   blackb     norm                4.99108E-06  +/-  1.02274E-06

copl+blackb:  The HighEcut is trying to go to the max limit of 7000.  There is no PL component to account for the high-energy data.  Not a good fit.  Only saved for plot. not bxa.

grbm+blackb+lpow:  parameters weren't stable enough to get errors.  Params looked good and fit the data well.  When it comes down to it, this should not be considered a good fit if errors aren't obtainable due to instability.
   1    1   grbm       alpha               -1.16803     +/-  0.108401     
   2    1   grbm       beta                -2.27354     +/-  4.85656E-02  
   3    1   grbm       tem        keV      1131.53      +/-  426.546      
   4    1   grbm       norm                1.18532E-02  +/-  8.79482E-04  
   5    2   blackb     kT         keV      40.7666      +/-  3.07964      
   6    2   blackb     norm                4.67441E-06  +/-  1.16067E-06  
   7    3   lpow       plIndex    NONE     -1.84856     +/-  0.117211     
   8    3   lpow       norm                5.83729E-04  +/-  6.33709E-04

sbpl+blackb+lpow:  PL too steep and doesn't contribute.  It only contributes very little to high energy.  No errors.  When it comes down to it, this should not be considered a good fit if errors aren't obtainable due to instability.
   1    1   sbpl       alpha      NONE     -1.27544     +/-  2.88553E-02  
   2    1   sbpl       beta       NONE     -2.23861     +/-  2.66196E-02  
   3    1   sbpl       ebreak     keV      556.091      +/-  111.112      
   4    1   sbpl       norm                1.12661E-02  +/-  4.98627E-04  
   5    2   blackb     kT         keV      39.8756      +/-  2.10116      
   6    2   blackb     norm                5.18080E-06  +/-  1.02090E-06  
   7    3   lpow       plIndex    NONE     -0.708004    +/-  0.930856     
   8    3   lpow       norm                2.24958E-09  +/-  2.67769E-08

copl+blackb+lpow:  got good 1-sigma errors without flags.  LAT and LLE data don't fit the PL at high energies though and you can't level it out to -2.0 because the BB and COPL at lower energies won't allow it.  Not a very good fit.
   1    1   copl       cplIndex   NONE     -0.644507    +/-  0.141433     
   2    1   copl       highEcut   NONE     490.578      +/-  106.062      
   3    1   copl       norm                9.06888E-03  +/-  9.39549E-04  
   4    2   blackb     kT         keV      33.1943      +/-  2.28576      
   5    2   blackb     norm                1.02988E-05  +/-  2.69905E-06  
   6    3   lpow       plIndex    NONE     -1.82140     +/-  1.18075E-02  
   7    3   lpow       norm                3.26551E-03  +/-  2.52659E-04

