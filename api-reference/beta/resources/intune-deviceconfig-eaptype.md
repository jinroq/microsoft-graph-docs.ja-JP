---
title: eapType 列挙型
description: 拡張認証プロトコル (EAP) の構成の種類。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e894e10356711fd4522ff816750e986d8b8e57d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957810"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="aaa2d-103">eapType 列挙型</span><span class="sxs-lookup"><span data-stu-id="aaa2d-103">eapType enum type</span></span>

> <span data-ttu-id="aaa2d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aaa2d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aaa2d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aaa2d-107">拡張認証プロトコル (EAP) の構成の種類。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>
## <a name="members"></a><span data-ttu-id="aaa2d-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="aaa2d-108">Members</span></span>
|<span data-ttu-id="aaa2d-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="aaa2d-109">Member</span></span>|<span data-ttu-id="aaa2d-110">値</span><span class="sxs-lookup"><span data-stu-id="aaa2d-110">Value</span></span>|<span data-ttu-id="aaa2d-111">説明</span><span class="sxs-lookup"><span data-stu-id="aaa2d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaa2d-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="aaa2d-112">eapTls</span></span>|<span data-ttu-id="aaa2d-113">13</span><span class="sxs-lookup"><span data-stu-id="aaa2d-113">13</span></span>|<span data-ttu-id="aaa2d-114">EAP トランスポート層セキュリティ (EAP-TLS) です。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="aaa2d-115">飛躍的に向上</span><span class="sxs-lookup"><span data-stu-id="aaa2d-115">leap</span></span>|<span data-ttu-id="aaa2d-116">17</span><span class="sxs-lookup"><span data-stu-id="aaa2d-116">17</span></span>|<span data-ttu-id="aaa2d-117">軽量の拡張認証プロトコル (LEAP)。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="aaa2d-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="aaa2d-118">eapSim</span></span>|<span data-ttu-id="aaa2d-119">18</span><span class="sxs-lookup"><span data-stu-id="aaa2d-119">18</span></span>|<span data-ttu-id="aaa2d-120">GSM サブスクライバー識別モジュール (EAP-SIM) の EAP です。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="aaa2d-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="aaa2d-121">eapTtls</span></span>|<span data-ttu-id="aaa2d-122">21</span><span class="sxs-lookup"><span data-stu-id="aaa2d-122">21</span></span>|<span data-ttu-id="aaa2d-123">EAP トンネルのトランスポート層セキュリティ (EAP-TTLS)。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="aaa2d-124">peap</span><span class="sxs-lookup"><span data-stu-id="aaa2d-124">peap</span></span>|<span data-ttu-id="aaa2d-125">25</span><span class="sxs-lookup"><span data-stu-id="aaa2d-125">25</span></span>|<span data-ttu-id="aaa2d-126">拡張認証プロトコル (PEAP) を保護します。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="aaa2d-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="aaa2d-127">eapFast</span></span>|<span data-ttu-id="aaa2d-128">43</span><span class="sxs-lookup"><span data-stu-id="aaa2d-128">43</span></span>|<span data-ttu-id="aaa2d-129">セキュリティで保護されたトンネル (EAP-FAST) を使用して EAP の柔軟な認証です。</span><span class="sxs-lookup"><span data-stu-id="aaa2d-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|





