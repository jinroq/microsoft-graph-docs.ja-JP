---
title: eapType 列挙型
description: 拡張認証プロトコル (EAP) の構成の種類。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 268a3190b06834d24c63d7ca5117a00fe7dc70d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405829"
---
# <a name="eaptype-enum-type"></a><span data-ttu-id="df10a-103">eapType 列挙型</span><span class="sxs-lookup"><span data-stu-id="df10a-103">eapType enum type</span></span>

> <span data-ttu-id="df10a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df10a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df10a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df10a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df10a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df10a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df10a-107">拡張認証プロトコル (EAP) の構成の種類。</span><span class="sxs-lookup"><span data-stu-id="df10a-107">Extensible Authentication Protocol (EAP) configuration types.</span></span>

## <a name="members"></a><span data-ttu-id="df10a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="df10a-108">Members</span></span>
|<span data-ttu-id="df10a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="df10a-109">Member</span></span>|<span data-ttu-id="df10a-110">値</span><span class="sxs-lookup"><span data-stu-id="df10a-110">Value</span></span>|<span data-ttu-id="df10a-111">説明</span><span class="sxs-lookup"><span data-stu-id="df10a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df10a-112">eapTls</span><span class="sxs-lookup"><span data-stu-id="df10a-112">eapTls</span></span>|<span data-ttu-id="df10a-113">13</span><span class="sxs-lookup"><span data-stu-id="df10a-113">13</span></span>|<span data-ttu-id="df10a-114">EAP トランスポート層セキュリティ (EAP-TLS) です。</span><span class="sxs-lookup"><span data-stu-id="df10a-114">EAP-Transport Layer Security (EAP-TLS).</span></span>|
|<span data-ttu-id="df10a-115">飛躍的に向上</span><span class="sxs-lookup"><span data-stu-id="df10a-115">leap</span></span>|<span data-ttu-id="df10a-116">17</span><span class="sxs-lookup"><span data-stu-id="df10a-116">17</span></span>|<span data-ttu-id="df10a-117">軽量の拡張認証プロトコル (LEAP)。</span><span class="sxs-lookup"><span data-stu-id="df10a-117">Lightweight Extensible Authentication Protocol (LEAP).</span></span>|
|<span data-ttu-id="df10a-118">eapSim</span><span class="sxs-lookup"><span data-stu-id="df10a-118">eapSim</span></span>|<span data-ttu-id="df10a-119">18</span><span class="sxs-lookup"><span data-stu-id="df10a-119">18</span></span>|<span data-ttu-id="df10a-120">GSM サブスクライバー識別モジュール (EAP-SIM) の EAP です。</span><span class="sxs-lookup"><span data-stu-id="df10a-120">EAP for GSM Subscriber Identity Module (EAP-SIM).</span></span>|
|<span data-ttu-id="df10a-121">eapTtls</span><span class="sxs-lookup"><span data-stu-id="df10a-121">eapTtls</span></span>|<span data-ttu-id="df10a-122">21</span><span class="sxs-lookup"><span data-stu-id="df10a-122">21</span></span>|<span data-ttu-id="df10a-123">EAP トンネルのトランスポート層セキュリティ (EAP-TTLS)。</span><span class="sxs-lookup"><span data-stu-id="df10a-123">EAP-Tunneled Transport Layer Security (EAP-TTLS).</span></span>|
|<span data-ttu-id="df10a-124">peap</span><span class="sxs-lookup"><span data-stu-id="df10a-124">peap</span></span>|<span data-ttu-id="df10a-125">25</span><span class="sxs-lookup"><span data-stu-id="df10a-125">25</span></span>|<span data-ttu-id="df10a-126">拡張認証プロトコル (PEAP) を保護します。</span><span class="sxs-lookup"><span data-stu-id="df10a-126">Protected Extensible Authentication Protocol (PEAP).</span></span>|
|<span data-ttu-id="df10a-127">eapFast</span><span class="sxs-lookup"><span data-stu-id="df10a-127">eapFast</span></span>|<span data-ttu-id="df10a-128">43</span><span class="sxs-lookup"><span data-stu-id="df10a-128">43</span></span>|<span data-ttu-id="df10a-129">セキュリティで保護されたトンネル (EAP-FAST) を使用して EAP の柔軟な認証です。</span><span class="sxs-lookup"><span data-stu-id="df10a-129">EAP-Flexible Authentication via Secure Tunneling (EAP-FAST).</span></span>|




