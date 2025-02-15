# Personalized Movie Recommender

This repository builded top of the [Personalized Feed](https://github.com/andthattoo/personalized-rss-feed) repository. Frontend developed with [Streamlit](https://github.com/streamlit/streamlit), Recommendation engine developed with [Firstbatch](https://github.com/firstbatchxyz/firstbatch-sdk).

# Features


- **Adaptive Conversations**:  Our chatbot learns from your previous interactions with movies and tailors the conversation accordingly.
- **News Content Integration**: Engage with movie content that you like, and the chatbot adapts!
- **Modern Interface**: Dark-themed, sleek design ensures an enjoyable user experience.

# How It Works

Once you interacted with any movie, chatbot will provide you personalized recommendations immediately while ensuring an exploration space for you to discover new tastes.

[FirstBatch SDK Documentation](https://firstbatch.gitbook.io/firstbatch-sdk/get-started/introduction)

## Setup

1. Clone the repository:
   ```bash
   git clone git@github.com:aktasbatuhan/personalized-movie-recommender.git
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up your API keys in the `st.secrets` configuration. Ensure you have API keys for both FirstBatch and Pinecone. A secrets.toml example:
    ```toml
   
    "custom_algo_id" = "[algo_id]"
    "pinecone_index"="[pinecone_index_name]"
    "firstbatch_db_name"="[firstbatch_db]"
    "embedding_size"="[embbedding_size_of_vectors]"
   
    [api]
    "pinecone_api_key"="[pinecone_key]"
    "pinecone_env"="[pinecone_env]"
    "firstbatch_api_key"="[firstbatch_key]"

    ```

4. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```

# Feedback & Contributions
We value your feedback and contributions. If you find a bug or have a feature request, please open an issue. Pull requests are also welcome!
