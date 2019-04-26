---
title: eaptype 列挙型
description: 拡張認証プロトコル (EAP) 構成の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c0fea3bed512c98cd26488a7703554ac6c600f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567138"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="7c0dd-103">eaptype 列挙型</span><span class="sxs-lookup"><span data-stu-id="7c0dd-103">eapType enum type</span></span>

> <span data-ttu-id="7c0dd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c0dd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c0dd-106">拡張認証プロトコル (EAP) 構成の種類。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-106">Extensible Authentication Protocol (EAP) configuration types.</span></span>

## <a name="members"></a><span data-ttu-id="7c0dd-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="7c0dd-107">Members</span></span>
|<span data-ttu-id="7c0dd-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="7c0dd-108">Member</span></span>|<span data-ttu-id="7c0dd-109">値</span><span class="sxs-lookup"><span data-stu-id="7c0dd-109">Value</span></span>|<span data-ttu-id="7c0dd-110">説明</span><span class="sxs-lookup"><span data-stu-id="7c0dd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c0dd-111">eaptls</span><span class="sxs-lookup"><span data-stu-id="7c0dd-111">eapTls</span></span>|<span data-ttu-id="7c0dd-112">13 </span><span class="sxs-lookup"><span data-stu-id="7c0dd-112">13</span></span>|<span data-ttu-id="7c0dd-113">eap-トランスポート層セキュリティ (eap-tls)。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-113">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="7c0dd-114">クリデンシャル</span><span class="sxs-lookup"><span data-stu-id="7c0dd-114">leap</span></span>|<span data-ttu-id="7c0dd-115">17 </span><span class="sxs-lookup"><span data-stu-id="7c0dd-115">17</span></span>|<span data-ttu-id="7c0dd-116">軽量の拡張認証プロトコル (LEAP)。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-116">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="7c0dd-117">eapsim</span><span class="sxs-lookup"><span data-stu-id="7c0dd-117">eapSim</span></span>|<span data-ttu-id="7c0dd-118">18 </span><span class="sxs-lookup"><span data-stu-id="7c0dd-118">18</span></span>|<span data-ttu-id="7c0dd-119">GSM サブスクライバー id モジュール (eap-SIM) の EAP。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-119">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="7c0dd-120">eapttls</span><span class="sxs-lookup"><span data-stu-id="7c0dd-120">eapTtls</span></span>|<span data-ttu-id="7c0dd-121">21</span><span class="sxs-lookup"><span data-stu-id="7c0dd-121">21</span></span>|<span data-ttu-id="7c0dd-122">eap トンネリングトランスポート層セキュリティ (eap-tls)。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-122">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="7c0dd-123">peap-gtc</span><span class="sxs-lookup"><span data-stu-id="7c0dd-123">peap</span></span>|<span data-ttu-id="7c0dd-124">まで</span><span class="sxs-lookup"><span data-stu-id="7c0dd-124">25</span></span>|<span data-ttu-id="7c0dd-125">保護された拡張認証プロトコル (PEAP)。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-125">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="7c0dd-126">eapfast</span><span class="sxs-lookup"><span data-stu-id="7c0dd-126">eapFast</span></span>|<span data-ttu-id="7c0dd-127">43</span><span class="sxs-lookup"><span data-stu-id="7c0dd-127">43</span></span>|<span data-ttu-id="7c0dd-128">セキュリティで保護されたトンネリング (eap-fast) 経由の eap による柔軟な認証。</span><span class="sxs-lookup"><span data-stu-id="7c0dd-128">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





