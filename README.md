# EarlyAD_DiagnosisUsingSpeech_and_Transcript
We developed a real time system for early diagnosis of AD using speech and transcript analysis. In progres...

Early detection of Alzheimer's disease (AD) is crucial for timely intervention and management. Traditional diagnostic methods often rely on manual assessments and structured data formats, which may not be conducive to real-time analysis. In this study, we present a novel, real-time web application that integrates acoustic and linguistic analyses of spontaneous speech to detect early signs of AD. Utilizing AssemblyAI's streaming transcription API, our system captures live speech and transcribes it in real-time, eliminating the need for pre-recorded .CHAT files. Acoustic features are extracted using the Wav2Vec2.0 model, followed by feature importance analysis through Random Forest classifiers and dimensionality reduction via Principal Component Analysis (PCA). For linguistic analysis, we combine [CLS] token embeddings from fine-tuned BERT models with Term Frequency-Inverse Document Frequency (TF-IDF) vectors to capture both contextual and frequency-based linguistic features. These features are then processed using PCA to streamline the dataset. The classification is performed using a soft-voting ensemble comprising Logistic Regression, Support Vector Machines, Random Forest, and XGBoost classifiers. Our approach demonstrates high accuracy and robustness in detecting linguistic and acoustic markers associated with early-stage AD. By facilitating real-time analysis and eliminating dependencies on structured data formats, this system offers a scalable and accessible tool for early AD detection, with potential applications in clinical and home settings.
