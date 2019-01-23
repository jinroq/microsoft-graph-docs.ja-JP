---
title: diagnosticDataSubmissionMode 列挙型
description: ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422258"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="783da-103">diagnosticDataSubmissionMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="783da-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="783da-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="783da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="783da-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="783da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="783da-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="783da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="783da-107">ワトソンなど、診断および利用状況の遠隔測定データを送信するデバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="783da-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="783da-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="783da-108">Members</span></span>
|<span data-ttu-id="783da-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="783da-109">Member</span></span>|<span data-ttu-id="783da-110">値</span><span class="sxs-lookup"><span data-stu-id="783da-110">Value</span></span>|<span data-ttu-id="783da-111">説明</span><span class="sxs-lookup"><span data-stu-id="783da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="783da-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="783da-112">userDefined</span></span>|<span data-ttu-id="783da-113">0</span><span class="sxs-lookup"><span data-stu-id="783da-113">0</span></span>|<span data-ttu-id="783da-114">設定するユーザーを許可します。</span><span class="sxs-lookup"><span data-stu-id="783da-114">Allow the user to set.</span></span>|
|<span data-ttu-id="783da-115">none</span><span class="sxs-lookup"><span data-stu-id="783da-115">none</span></span>|<span data-ttu-id="783da-116">1</span><span class="sxs-lookup"><span data-stu-id="783da-116">1</span></span>|<span data-ttu-id="783da-117">OS コンポーネントからは、遠隔測定データは送信されません。</span><span class="sxs-lookup"><span data-stu-id="783da-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="783da-118">注: この値は、エンタープライズとサーバのデバイスに適用されるのみです。</span><span class="sxs-lookup"><span data-stu-id="783da-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="783da-119">その他のデバイスでこの設定を使用して、1 の値を設定するのと同じです。</span><span class="sxs-lookup"><span data-stu-id="783da-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="783da-120">基本的な</span><span class="sxs-lookup"><span data-stu-id="783da-120">basic</span></span>|<span data-ttu-id="783da-121">2</span><span class="sxs-lookup"><span data-stu-id="783da-121">2</span></span>|<span data-ttu-id="783da-122">基本的な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="783da-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="783da-123">強化</span><span class="sxs-lookup"><span data-stu-id="783da-123">enhanced</span></span>|<span data-ttu-id="783da-124">3</span><span class="sxs-lookup"><span data-stu-id="783da-124">3</span></span>|<span data-ttu-id="783da-125">送信には、使用状況と情報のデータを含む遠隔測定データが強化されています。</span><span class="sxs-lookup"><span data-stu-id="783da-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="783da-126">フル</span><span class="sxs-lookup"><span data-stu-id="783da-126">full</span></span>|<span data-ttu-id="783da-127">4</span><span class="sxs-lookup"><span data-stu-id="783da-127">4</span></span>|<span data-ttu-id="783da-128">システム状態などの診断データを含む完全な遠隔測定データを送信します。</span><span class="sxs-lookup"><span data-stu-id="783da-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




