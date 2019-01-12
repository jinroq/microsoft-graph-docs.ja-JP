---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: d1ba4d2cd9be740b23502ec4c0154caa2be07f3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948531"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="a84a1-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="a84a1-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="a84a1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a84a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a84a1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a84a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a84a1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a84a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a84a1-107">ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a84a1-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="a84a1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a84a1-108">Members</span></span>
|<span data-ttu-id="a84a1-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="a84a1-109">Member</span></span>|<span data-ttu-id="a84a1-110">値</span><span class="sxs-lookup"><span data-stu-id="a84a1-110">Value</span></span>|<span data-ttu-id="a84a1-111">説明</span><span class="sxs-lookup"><span data-stu-id="a84a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a84a1-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="a84a1-112">userDefined</span></span>|<span data-ttu-id="a84a1-113">0</span><span class="sxs-lookup"><span data-stu-id="a84a1-113">0</span></span>|<span data-ttu-id="a84a1-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="a84a1-114">Allow the user to set.</span></span>|
|<span data-ttu-id="a84a1-115">none</span><span class="sxs-lookup"><span data-stu-id="a84a1-115">none</span></span>|<span data-ttu-id="a84a1-116">1</span><span class="sxs-lookup"><span data-stu-id="a84a1-116">1</span></span>|<span data-ttu-id="a84a1-117">OS コンポーネントからは、遠隔測定データは送信されません。</span><span class="sxs-lookup"><span data-stu-id="a84a1-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="a84a1-118">注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。</span><span class="sxs-lookup"><span data-stu-id="a84a1-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="a84a1-119">その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="a84a1-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="a84a1-120">基本的な</span><span class="sxs-lookup"><span data-stu-id="a84a1-120">basic</span></span>|<span data-ttu-id="a84a1-121">2</span><span class="sxs-lookup"><span data-stu-id="a84a1-121">2</span></span>|<span data-ttu-id="a84a1-122">基本的な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="a84a1-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="a84a1-123">強化</span><span class="sxs-lookup"><span data-stu-id="a84a1-123">enhanced</span></span>|<span data-ttu-id="a84a1-124">3</span><span class="sxs-lookup"><span data-stu-id="a84a1-124">3</span></span>|<span data-ttu-id="a84a1-125">送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。</span><span class="sxs-lookup"><span data-stu-id="a84a1-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="a84a1-126">フル</span><span class="sxs-lookup"><span data-stu-id="a84a1-126">full</span></span>|<span data-ttu-id="a84a1-127">4</span><span class="sxs-lookup"><span data-stu-id="a84a1-127">4</span></span>|<span data-ttu-id="a84a1-128">システム状態などの診断データを含む完全な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="a84a1-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





