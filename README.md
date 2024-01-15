# widget

import streamlit as st


def set_bg_hack_url():
    '''
    A function to unpack an image from url and set as bg.
    Returns
    -------
    The background.
    '''

    st.markdown(
        f"""
         <style>
         .stApp {{
             background: url("https://cdn.pixabay.com/photo/2020/06/19/22/33/wormhole-5319067_960_720.jpg");
             background-size: cover
         }}
         </style>
         """,
        unsafe_allow_html=True
    )

# Set up the iframe
iframe_html = """
<iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/1samlRVE4AvI9UJJYQ7XEU?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>"""

# Display the iframe in the Streamlit app
st.markdown(iframe_html, unsafe_allow_html=True)
