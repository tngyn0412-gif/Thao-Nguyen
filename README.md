import streamlit as st
import pandas as pd

# ==============================
# CẤU HÌNH TRANG
# ==============================

st.set_page_config(
    page_title="Tính lãi tiền gửi tiết kiệm",
    page_icon="💰",
    layout="centered"
)

# ==============================
# CSS
# ==============================

st.markdown("""
<style>
    .main-title {
        text-align: center;
        font-size: 32px;
        font-weight: bold;
        margin-bottom: 10px;
    }

    .sub-title {
        text-align: center;
        color: #666;
        margin-bottom: 30px;
    }

    .result-box {
        padding: 20px;
        border-radius: 12px;
        background-color: #f5f7fa;
        margin-bottom: 15px;
    }

    .result-title {
        font-size: 16px;
        color: #555;
    }

    .result-value {
        font-size: 24px;
        font-weight: bold;
    }
</style>
""", unsafe_allow_html=True)

# ==============================
# TIÊU ĐỀ
# ==============================

st.markdown(
    '<div class="main-title">💰 MÁY TÍNH LÃI
