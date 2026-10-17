# ISAC Waveform Design Breakthrough! Probabilistic Denoising Enhanced PDISAC Achieves Both Perception and Communication Performances [with MATLAB + Python Code]

ISAC Waveform Design Breakthrough! Probabilistic Denoising Enhanced PDISAC Achieves Both Perception and Communication Performance
In the development of 6G communication technology, Integrated Sensing and Communications (ISAC) has become a core research direction. The core challenge lies in designing waveforms that can simultaneously meet high distance-Doppler resolution (perception requirements) and high throughput (communication requirements). However, there is inherent conflict between perception and communication performance targets, making it difficult for traditional methods to achieve optimal balance. Recent research has proposed a novel framework for probabilistic denoising enhanced parameterized waveform design—PDISAC (Probabilistic Denoising ISAC), which perfectly solves the performance shortcomings of traditional methods under non-ideal channels and multi-objective scenarios. It also provides theoretical guarantees for ISAC system performance, outperforming classic matched filtering and traditional learning-based methods under low Signal-to-Noise Ratio (SNR).
Traditional Pain Points in ISAC Waveform Design:
1. Traditional Matched Filtering: Relies on fixed waveform parameters, performing suboptimally under unfavorable channel conditions and multi-objective perception scenarios, lacking flexibility to adapt to complex scenarios;
2. Learning-Based ISAC Methods: While capable of model learning to adapt to complex scenarios, lack strict theoretical performance guarantees, raising doubts about their reliability in engineering implementation.
To address these issues, the PDISAC framework integrates probabilistic machine learning with parameterized waveform design. It not only characterizes the system performance limits through theoretical derivation but also enhances perception and communication performance in real scenarios with lightweight networks, achieving a dual breakthrough of "theoretical guarantee + practical optimization."
Core Design of PDISAC: Probabilistic Denoising + Parameterized Waveform
The core of PDISAC is the establishment of a probabilistic denoising enhanced parameterized waveform design system. Centered around a lightweight probability denoising network (PDNet), it also completes theoretical analysis and engineering design. The core highlights are threefold:
1. Core Network: PDNet realizes high-quality RD heatmap generation. PDNet is a lightweight probability denoising network specifically designed for ISAC, which completes model training through time-frequency domain adversarial training, effectively generates high-quality distance-Doppler (RD) heatmaps, significantly enhances target discernibility under different waveform sequence lengths, and allows for more accurate perception in multi-target scenarios.
At the same time, PDNet adopts the "training-inference separation" architecture design: The training architecture includes encoder, extractor, and decoder modules to ensure the integrity of feature learning. The reasoning architecture removes the encoder, significantly reducing computational costs and reducing real-time inference latency, making it more suitable for engineering deployment.
2. Theoretical Support: Derivation of Closed-Form Expressions for Performance Limits
3. Scenario Compatibility: Analyzing the Perception-Communication Trade-off Affected by Sequence Length
III. PDISAC Technology Details: From System Model to Denoising Pipeline
Its waveform is completed in the time domain, divided into two core dimensions: fast and slow domains, with clear division of labor.
★  
Fast Domain: Used for estimating target distance, resolution is determined by the number of code chips.
★  
Slow-domain: Used to estimate the target Doppler (velocity), resolution is determined by the number of symbols.
At the same time, waveform transmission integrates PMCW waveform and BPSK symbols to achieve integrated waveform transmission of perception and communication.
2. The three-step denoising pipeline, combined with adversarial training to optimize the PDISAC design, has become a key factor in improving perception performance. The entire process is divided into three steps: preprocessing, training/inference, and post-processing. Adversarial training is also introduced to further optimize the denoising effect.
1  
Preprocessing: Convert time-frequency domain observation values into an RDT heatmap, serving as the input for PDNet (no need for matched filter processing, simplifying the process);
2  
Training/Inference: Denoise the data through the training/inference architecture of PDNet, and generate an optimized RD heatmap.
3  
Post-processing: Restore the time-frequency domain matched filter output from the optimized RD heatmap to prepare for subsequent parameter estimation.
Adversarial training serves as a supplementary optimization phase, further enhancing the denoising model's performance and making PDNet more effective in noise reduction under low SNR conditions.
3. Dual-method implementation of distance-Doppler parameter estimation PDISAC employs two methods: sequential estimator and constant false alarm rate (CFAR) to estimate the parameters of target distance and velocity, adapting to different scene requirements.
★  
Sequential Estimator: First detect the distance peak, then based on the distance peak detect the Doppler peak, completing parameter estimation in steps.
★  
CFAR: Directly mark potential targets based on RD heatmaps, complete the identification of UE and TE through blue circles. It is more suitable for rapid detection of multiple targets.
The study also verified the impact of resolution: the larger the values, the higher the resolution for distance and speed, providing a clear basis for waveform parameter tuning.
IV. PDISAC Experimental Verification: Comprehensive Leading Performance under Low SNR for verifying the performance of PDISAC, the research team conducted map-based channel simulations and compared them with traditional matched filtering and classic learning-based model DnCNN in multiple dimensions. The core verification results are as follows:
1  
Perception performance: Under low SNR, the CRLB of PDISAC is significantly better than that of the contrastive methods, and it has a better NMSE and MSE indicators, and higher accuracy in distance-velocity parameter estimation.
2  
Communication Performance: PDISAC ensures perception performance while achieving reliable communication performance, with BER (Bit Error Rate) and capacity indicators showing stable performance without significant loss.
3  
Robustness: Under different waveform sequence lengths, PDISAC can maintain excellent target distinguishability, far surpassing traditional methods.
In the experiment, the visual verification of PDNet denoising on perception performance was conducted through RD heatmap and denoising process distribution visualization. The precise marking of moving targets UE and TE after CFAR treatment fully demonstrates the effectiveness of PDISAC in multi-target scenarios.
V. Research Significance and Future Prospects
At the same time, PDNet's lightweight design and inference delay optimization have made this framework potential for engineering implementation. Its outstanding performance under low SNR also makes it suitable for more complex real communication perception scenarios.
In the future, this research direction can further revolve around network lightweightness, ultra-multiple target scenario adaptation, and dynamic channel adaptive optimization. This will make PDISAC more aligned with the actual deployment needs of 6G ISAC, promoting the practical application of integrated perception communication technology.

## Images

![ISAC waveform design breakthrough! Probabilistic denoising enhanced PDISAC that balances perception and communication dual performance [with MATLAB + Python code]](01.jpg)
![ISAC waveform design breakthrough! Probabilistic denoising enhanced PDISAC that balances perception and communication dual performance [with MATLAB + Python code]](02.jpg)
![ISAC waveform design breakthrough! Probabilistic denoising enhanced PDISAC that balances perception and communication dual performance [with MATLAB + Python code]](03.jpg)
![ISAC waveform design breakthrough! Probabilistic denoising enhanced PDISAC that balances perception and communication dual performance [with MATLAB + Python code]](04.jpg)
![ISAC waveform design breakthrough! Probabilistic denoising enhanced PDISAC that balances perception and communication dual performance [with MATLAB + Python code]](05.jpg)
![ISAC waveform design breakthrough! Probabilistic denoising enhanced PDISAC that balances perception and communication dual performance [with MATLAB + Python code]](06.jpg)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
