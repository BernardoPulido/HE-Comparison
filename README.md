# Towards Understanding Efficient Privacy-Preserving Homomorphic Comparison

Homomorphic Encryption (HE) emerges as a mechanism for expanding the scope of public cloud services for sensitive data processing. HE describes a special form of encryption with the capability of performing certain operations over ciphertexts without using the secret key. The information can be public without representing a risk of a data breach. The output of the calculated functions remains encrypted and maintains the input format. Its correctness relies on the homomorphism concept, where two groups in different spaces can be mapped. In this case, a homomorphic function applied to ciphertexts provides the same result (after decryption) as applying the function to the original unencrypted data.

However, high-demand solutions such as machine learning require efficient operations beyond HE additions and multiplications. The state-of-the-art solutions have been focused on implementing cryptographically compatible comparison and sign functions. In the paper (link to be added upon publication), we analyze the current homomorphic comparison methods across their strengths and weaknesses and present theoretical concepts, state-of-the-art techniques, challenges, opportunities, and open problems. We compare the efficiency, accuracy, and computational complexity of different homomorphic comparison approaches. This project includes the source code used in this study. 

The HE schemes and homomorphic operations were implemented using the open-source Simple Encrypted Arithmetic Library (SEAL) through the Python [TenSEAL](https://github.com/OpenMined/TenSEAL/) library. The ciphertext size, scheme performance, multiplicative depth, and security level directly depend on the security parameter settings. We adopt security settings specified in the [HE standard](https://HomomorphicEncryption.org/standard).

The project includes three Jupyter notebooks:
- BFV_CKKS schemes.ipynd: Primitives of BFV and CKKS HE schemes.  
- Interval_based_approximation_analysis.ipynb: Interval-based error analysis.
- Performance_accuracy_comparison_approaches.ipynb: Performance of the state-of-the-art fixed-precision numbers homomorphic comparison approaches.

For assistance with this source code, please contact us at lpulido@cicese.edu.mx
