---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
ms.openlocfilehash: b09a4bf334af5981c3ce6dabbab0ac64e2b24887
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023270"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="1dc61-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="1dc61-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="1dc61-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1dc61-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1dc61-105">ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="1dc61-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="1dc61-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="1dc61-106">Members</span></span>
|<span data-ttu-id="1dc61-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1dc61-107">Member</span></span>|<span data-ttu-id="1dc61-108">値</span><span class="sxs-lookup"><span data-stu-id="1dc61-108">Value</span></span>|<span data-ttu-id="1dc61-109">説明</span><span class="sxs-lookup"><span data-stu-id="1dc61-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dc61-110">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="1dc61-110">userDefined</span></span>|<span data-ttu-id="1dc61-111">0</span><span class="sxs-lookup"><span data-stu-id="1dc61-111">0</span></span>|<span data-ttu-id="1dc61-112">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="1dc61-112">Allow the user to set.</span></span>|
|<span data-ttu-id="1dc61-113">none</span><span class="sxs-lookup"><span data-stu-id="1dc61-113">none</span></span>|<span data-ttu-id="1dc61-114">1</span><span class="sxs-lookup"><span data-stu-id="1dc61-114">1</span></span>|<span data-ttu-id="1dc61-115">OS コンポーネントからは、遠隔測定データは送信されません。</span><span class="sxs-lookup"><span data-stu-id="1dc61-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="1dc61-116">注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。</span><span class="sxs-lookup"><span data-stu-id="1dc61-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="1dc61-117">その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="1dc61-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="1dc61-118">基本的な</span><span class="sxs-lookup"><span data-stu-id="1dc61-118">basic</span></span>|<span data-ttu-id="1dc61-119">2</span><span class="sxs-lookup"><span data-stu-id="1dc61-119">2</span></span>|<span data-ttu-id="1dc61-120">基本的な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="1dc61-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="1dc61-121">強化</span><span class="sxs-lookup"><span data-stu-id="1dc61-121">enhanced</span></span>|<span data-ttu-id="1dc61-122">3</span><span class="sxs-lookup"><span data-stu-id="1dc61-122">3</span></span>|<span data-ttu-id="1dc61-123">送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。</span><span class="sxs-lookup"><span data-stu-id="1dc61-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="1dc61-124">フル</span><span class="sxs-lookup"><span data-stu-id="1dc61-124">full</span></span>|<span data-ttu-id="1dc61-125">4</span><span class="sxs-lookup"><span data-stu-id="1dc61-125">4</span></span>|<span data-ttu-id="1dc61-126">システム状態などの診断データを含む完全な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="1dc61-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



