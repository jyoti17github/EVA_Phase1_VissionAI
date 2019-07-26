## Receptive field calulation of 45 from 29 at layer7 --  page 21 (https://arxiv.org/pdf/1701.03056.pdf)
it is deduced from paper, (kernals) K = 3, (stride) S = 2,(jump at layer 7) J = 8 
and rf formula is--

Rf = rf(input) + (K-1)J  , where rf(input) receptive field input to the layer

      Rf = 29 + (3-1)8   # rf(input) is previous layer receptive field and in this case it is 29
      
      Rf = 29 + 16
      
      Rf = 45  
