# cs-smaf
training a dictionary using compressed sensing and two algorithems
clearly's algorithem:



i) use non-negative factorization to derive U and W  from X the gene expression matrix


ii) use X,W and lasso optimization: ||X.T-W.T U.T||l2+c||U.T||l1 to create a sparse U


iii) use X,U,Orthogonal Matching Pursuit (OMP) to optimize : ||X-UW||l2^2 s.t ||W||l0<n

                                                                                        
 iv) repeat the process until U and W converges
 
                                                                                        
  my algorithem:
                                                                                     
  i) use non-negative factorization to derive U and W  from X the gene expression matrix

                                                                                        
   ii) use X,W and lasso optimization: ||X.T-W.T U.T||l2+c||U.T||l1 to create a sparse U                                                                                        

                                                                                        
   iii)use X,U and lasso optimization: ||X-UW||l2+c||W||l1 to create a sparse W

                                                                                        
   iv)repeat the process if needed

                                                                                        
                                                                                        
    my algorithem remains untested 
                                                        
                                                                          
