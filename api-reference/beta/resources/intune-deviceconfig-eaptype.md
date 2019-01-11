---
title: eapType 列挙型
description: 拡張認証プロトコル (EAP) の構成の種類。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 92c1cddd42f16556cbba51be7eb06a0f75c537a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828897"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="4c120-103">eapType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4c120-103">eapType enum type</span></span>

> <span data-ttu-id="4c120-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c120-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c120-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c120-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c120-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c120-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c120-107">拡張認証プロトコル (EAP) の構成の種類。</span><span class="sxs-lookup"><span data-stu-id="4c120-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="4c120-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4c120-108">Members</span></span>
|<span data-ttu-id="4c120-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4c120-109">Member</span></span>|<span data-ttu-id="4c120-110">値</span><span class="sxs-lookup"><span data-stu-id="4c120-110">Value</span></span>|<span data-ttu-id="4c120-111">説明</span><span class="sxs-lookup"><span data-stu-id="4c120-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c120-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="4c120-112">eapTls</span></span>|<span data-ttu-id="4c120-113">13</span><span class="sxs-lookup"><span data-stu-id="4c120-113">13</span></span>|<span data-ttu-id="4c120-114">EAP トランスポート層セキュリティ (EAP-TLS) です。</span><span class="sxs-lookup"><span data-stu-id="4c120-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="4c120-115">飛躍的に向上</span><span class="sxs-lookup"><span data-stu-id="4c120-115">leap</span></span>|<span data-ttu-id="4c120-116">17</span><span class="sxs-lookup"><span data-stu-id="4c120-116">17</span></span>|<span data-ttu-id="4c120-117">軽量の拡張認証プロトコル (LEAP)。</span><span class="sxs-lookup"><span data-stu-id="4c120-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="4c120-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="4c120-118">eapSim</span></span>|<span data-ttu-id="4c120-119">18</span><span class="sxs-lookup"><span data-stu-id="4c120-119">18</span></span>|<span data-ttu-id="4c120-120">GSM サブスクライバー識別モジュール (EAP-SIM) の EAP です。</span><span class="sxs-lookup"><span data-stu-id="4c120-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="4c120-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="4c120-121">eapTtls</span></span>|<span data-ttu-id="4c120-122">21</span><span class="sxs-lookup"><span data-stu-id="4c120-122">21</span></span>|<span data-ttu-id="4c120-123">EAP トンネルのトランスポート層セキュリティ (EAP-TTLS)。</span><span class="sxs-lookup"><span data-stu-id="4c120-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="4c120-124">peap</span><span class="sxs-lookup"><span data-stu-id="4c120-124">peap</span></span>|<span data-ttu-id="4c120-125">25</span><span class="sxs-lookup"><span data-stu-id="4c120-125">25</span></span>|<span data-ttu-id="4c120-126">拡張認証プロトコル (PEAP) を保護します。</span><span class="sxs-lookup"><span data-stu-id="4c120-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="4c120-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="4c120-127">eapFast</span></span>|<span data-ttu-id="4c120-128">43</span><span class="sxs-lookup"><span data-stu-id="4c120-128">43</span></span>|<span data-ttu-id="4c120-129">セキュリティで保護されたトンネル (EAP-FAST) を使用して EAP の柔軟な認証です。</span><span class="sxs-lookup"><span data-stu-id="4c120-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





