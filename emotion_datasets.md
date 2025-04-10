# Datasets for Emotion Recognition Training

## Overview

This document identifies and describes optimal datasets for training 2o8's emotion recognition capabilities. These datasets have been selected to provide comprehensive coverage of different emotional expressions, contexts, and cultural variations.

## Text-Based Emotion Datasets

### 1. General Emotion Classification Datasets

#### GoEmotions
- **Description**: Large-scale dataset of 58k Reddit comments labeled with 27 emotion categories
- **Size**: 58,000 comments
- **Labels**: 27 emotion categories including admiration, amusement, anger, annoyance, approval, caring, confusion, curiosity, desire, disappointment, disapproval, disgust, embarrassment, excitement, fear, gratitude, grief, joy, love, nervousness, optimism, pride, realization, relief, remorse, sadness, surprise
- **Advantages**: Fine-grained emotion categories, natural social media text, multiple emotions per comment
- **Source**: Google Research

#### EmoBank
- **Description**: Corpus of 10k English sentences annotated with emotion dimensions
- **Size**: 10,000 sentences
- **Labels**: Valence, Arousal, Dominance (VAD) dimensions on a 1-5 scale
- **Advantages**: Dimensional emotion representation, double perspective (writer's and reader's emotions)
- **Source**: Saarland University

#### ISEAR (International Survey on Emotion Antecedents and Reactions)
- **Description**: Self-reported emotional situations from 3,000 respondents in 37 countries
- **Size**: 7,665 reports
- **Labels**: 7 emotion categories (joy, fear, anger, sadness, disgust, shame, guilt)
- **Advantages**: Cross-cultural data, real emotional experiences, contextual information
- **Source**: Swiss Center for Affective Sciences

### 2. Conversational Emotion Datasets

#### EmpatheticDialogues
- **Description**: 25k conversations grounded in emotional situations
- **Size**: 24,850 conversations
- **Labels**: 32 emotion categories
- **Advantages**: Conversational context, empathetic responses, diverse situations
- **Source**: Facebook AI Research

#### DailyDialog
- **Description**: Multi-turn dialogues reflecting daily communication
- **Size**: 13,118 dialogues
- **Labels**: 7 emotion categories (anger, disgust, fear, happiness, sadness, surprise, no emotion)
- **Advantages**: Multi-turn conversations, natural daily communication, emotion flow
- **Source**: City University of Hong Kong

#### EmotionLines/MELD (Multimodal EmotionLines Dataset)
- **Description**: Dialogues from Friends TV show with emotion labels
- **Size**: 1,433 dialogues, 13,708 utterances
- **Labels**: 7 emotion categories (anger, disgust, fear, joy, neutral, sadness, surprise)
- **Advantages**: Conversational context, sequential emotions, multimodal option (text + audio + visual)
- **Source**: National Taiwan University

### 3. Fine-tuning Specific Datasets

#### AAID (Affective Analysis Instruction Dataset)
- **Description**: Instruction dataset for affective analysis from EmoLLMs paper
- **Size**: 234,000 samples
- **Tasks**: 3 classification tasks and 2 regression tasks
- **Advantages**: Designed for instruction tuning, comprehensive affective analysis
- **Source**: EmoLLMs project

#### AEB (Affective Evaluation Benchmark)
- **Description**: Benchmark for evaluating affective analysis capabilities
- **Size**: Multiple test sets covering 8 regression tasks and 6 classification tasks
- **Advantages**: Diverse sources and domains, comprehensive evaluation
- **Source**: EmoLLMs project

#### SemEval Emotion Tasks Datasets
- **Description**: Various datasets from SemEval emotion analysis tasks
- **Size**: Varies by task
- **Labels**: Various emotion taxonomies
- **Advantages**: Standardized evaluation, diverse text types
- **Source**: SemEval competitions

## Specialized Emotion Datasets

### 1. Cultural and Multilingual Emotion Datasets

#### NRC Emotion Lexicon
- **Description**: Word-emotion association lexicon in multiple languages
- **Size**: 14,182 words in English, translated to 100+ languages
- **Labels**: 8 emotions (anger, fear, anticipation, trust, surprise, sadness, joy, disgust) and 2 sentiments
- **Advantages**: Multilingual, lexicon-based, Plutchik's emotion model
- **Source**: National Research Council Canada

#### Multilingual Emotion Dataset
- **Description**: Tweets in 6 languages with emotion labels
- **Size**: ~100k tweets across languages
- **Labels**: 4-8 emotion categories depending on language
- **Advantages**: Cross-lingual comparison, natural social media text
- **Source**: Various academic sources

### 2. Complex Emotion Datasets

#### CARER (Context-Aware Emotion Recognition)
- **Description**: Dataset focusing on contextual emotion recognition
- **Size**: 20,000 context-emotion pairs
- **Labels**: 6 basic emotions plus additional complex emotions
- **Advantages**: Context-dependent emotions, ambiguous cases
- **Source**: Academic research

#### Sarcasm Detection Datasets
- **Description**: Various datasets for sarcasm and irony detection
- **Size**: Varies by dataset
- **Labels**: Sarcasm/irony presence, sometimes with emotion labels
- **Advantages**: Challenging cases for emotion recognition, implicit emotions
- **Source**: Various academic sources

### 3. Therapeutic and Mental Health Datasets

#### Counseling Conversations
- **Description**: Anonymized therapy session transcripts
- **Size**: Varies by source
- **Labels**: Emotional states, therapeutic interventions
- **Advantages**: Professional emotional support examples, complex emotional situations
- **Source**: Various research institutions with ethical approval

#### Mental Health Forums
- **Description**: Anonymized posts from mental health support forums
- **Size**: Varies by source
- **Labels**: Emotional states, mental health conditions
- **Advantages**: Real emotional expressions, supportive responses
- **Source**: Various research datasets with ethical approval

## Synthetic and Augmented Datasets

### 1. Emotion Variation Datasets
- **Description**: Synthetic variations of text with different emotional tones
- **Generation Method**: Controlled text generation with emotion conditioning
- **Advantages**: Controlled variation, balanced emotion categories

### 2. Complex Emotional Blend Datasets
- **Description**: Synthetic examples with complex emotional blends
- **Generation Method**: Mixing multiple emotion categories with varying intensities
- **Advantages**: Training for ambiguous and mixed emotions

### 3. Adversarial Emotion Examples
- **Description**: Challenging cases for emotion recognition
- **Generation Method**: Adversarial generation targeting emotion recognition weaknesses
- **Advantages**: Improving robustness of emotion recognition

## Data Integration Strategy

### 1. Multi-Source Training
- Combine complementary datasets to cover the full spectrum of emotions
- Balance categorical and dimensional emotion representations
- Ensure coverage of different text types and contexts

### 2. Data Augmentation Techniques
- Back-translation for linguistic variation
- Synonym replacement preserving emotional content
- Contextual augmentation with emotion preservation

### 3. Balanced Sampling Strategy
- Stratified sampling to balance emotion categories
- Curriculum learning from basic to complex emotions
- Active learning to focus on challenging cases

This comprehensive collection of datasets will provide the foundation for training 2o8 to recognize and understand the full spectrum of human emotions across different contexts, cultures, and expression styles.
