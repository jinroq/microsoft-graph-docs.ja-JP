---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
localization_priority: Normal
ms.openlocfilehash: 1654e9c5c94fd79bbda0d77ef84101fb9fb92d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812783"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="9c108-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="9c108-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="9c108-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c108-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c108-105">ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="9c108-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="9c108-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c108-106">Members</span></span>
|<span data-ttu-id="9c108-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9c108-107">Member</span></span>|<span data-ttu-id="9c108-108">値</span><span class="sxs-lookup"><span data-stu-id="9c108-108">Value</span></span>|<span data-ttu-id="9c108-109">説明</span><span class="sxs-lookup"><span data-stu-id="9c108-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c108-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="9c108-110">userDefined</span></span>|<span data-ttu-id="9c108-111">0</span><span class="sxs-lookup"><span data-stu-id="9c108-111">0</span></span>|<span data-ttu-id="9c108-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="9c108-112">Allow the user to set.</span></span>|
|<span data-ttu-id="9c108-113">none</span><span class="sxs-lookup"><span data-stu-id="9c108-113">none</span></span>|<span data-ttu-id="9c108-114">1</span><span class="sxs-lookup"><span data-stu-id="9c108-114">1</span></span>|<span data-ttu-id="9c108-115">OS コンポーネントからは、遠隔測定データは送信されません。</span><span class="sxs-lookup"><span data-stu-id="9c108-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="9c108-116">注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。</span><span class="sxs-lookup"><span data-stu-id="9c108-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="9c108-117">その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="9c108-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="9c108-118">基本的な</span><span class="sxs-lookup"><span data-stu-id="9c108-118">basic</span></span>|<span data-ttu-id="9c108-119">2</span><span class="sxs-lookup"><span data-stu-id="9c108-119">2</span></span>|<span data-ttu-id="9c108-120">基本的な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="9c108-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="9c108-121">強化</span><span class="sxs-lookup"><span data-stu-id="9c108-121">enhanced</span></span>|<span data-ttu-id="9c108-122">3</span><span class="sxs-lookup"><span data-stu-id="9c108-122">3</span></span>|<span data-ttu-id="9c108-123">送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。</span><span class="sxs-lookup"><span data-stu-id="9c108-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="9c108-124">フル</span><span class="sxs-lookup"><span data-stu-id="9c108-124">full</span></span>|<span data-ttu-id="9c108-125">4</span><span class="sxs-lookup"><span data-stu-id="9c108-125">4</span></span>|<span data-ttu-id="9c108-126">システム状態などの診断データを含む完全な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="9c108-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



