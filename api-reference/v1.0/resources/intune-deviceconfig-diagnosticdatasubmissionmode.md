---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912947"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="ac352-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="ac352-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="ac352-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac352-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac352-105">ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="ac352-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="ac352-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="ac352-106">Members</span></span>
|<span data-ttu-id="ac352-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ac352-107">Member</span></span>|<span data-ttu-id="ac352-108">値</span><span class="sxs-lookup"><span data-stu-id="ac352-108">Value</span></span>|<span data-ttu-id="ac352-109">説明</span><span class="sxs-lookup"><span data-stu-id="ac352-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac352-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="ac352-110">userDefined</span></span>|<span data-ttu-id="ac352-111">0</span><span class="sxs-lookup"><span data-stu-id="ac352-111">0</span></span>|<span data-ttu-id="ac352-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="ac352-112">Allow the user to set.</span></span>|
|<span data-ttu-id="ac352-113">none</span><span class="sxs-lookup"><span data-stu-id="ac352-113">none</span></span>|<span data-ttu-id="ac352-114">1</span><span class="sxs-lookup"><span data-stu-id="ac352-114">1</span></span>|<span data-ttu-id="ac352-115">OS コンポーネントからは、遠隔測定データは送信されません。</span><span class="sxs-lookup"><span data-stu-id="ac352-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="ac352-116">注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。</span><span class="sxs-lookup"><span data-stu-id="ac352-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="ac352-117">その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="ac352-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="ac352-118">基本的な</span><span class="sxs-lookup"><span data-stu-id="ac352-118">basic</span></span>|<span data-ttu-id="ac352-119">2</span><span class="sxs-lookup"><span data-stu-id="ac352-119">2</span></span>|<span data-ttu-id="ac352-120">基本的な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="ac352-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="ac352-121">強化</span><span class="sxs-lookup"><span data-stu-id="ac352-121">enhanced</span></span>|<span data-ttu-id="ac352-122">3</span><span class="sxs-lookup"><span data-stu-id="ac352-122">3</span></span>|<span data-ttu-id="ac352-123">送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。</span><span class="sxs-lookup"><span data-stu-id="ac352-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="ac352-124">フル</span><span class="sxs-lookup"><span data-stu-id="ac352-124">full</span></span>|<span data-ttu-id="ac352-125">4</span><span class="sxs-lookup"><span data-stu-id="ac352-125">4</span></span>|<span data-ttu-id="ac352-126">システム状態などの診断データを含む完全な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="ac352-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



