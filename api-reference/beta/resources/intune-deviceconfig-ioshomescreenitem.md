---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc351025f81931ac7deb33bec9be973a513a51fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809955"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="527f5-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="527f5-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="527f5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="527f5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="527f5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="527f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="527f5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="527f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="527f5-107">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="527f5-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="527f5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="527f5-108">Properties</span></span>
|<span data-ttu-id="527f5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="527f5-109">Property</span></span>|<span data-ttu-id="527f5-110">種類</span><span class="sxs-lookup"><span data-stu-id="527f5-110">Type</span></span>|<span data-ttu-id="527f5-111">説明</span><span class="sxs-lookup"><span data-stu-id="527f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="527f5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="527f5-112">displayName</span></span>|<span data-ttu-id="527f5-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="527f5-113">String</span></span>|<span data-ttu-id="527f5-114">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="527f5-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="527f5-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="527f5-115">Relationships</span></span>
<span data-ttu-id="527f5-116">なし</span><span class="sxs-lookup"><span data-stu-id="527f5-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="527f5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="527f5-117">JSON Representation</span></span>
<span data-ttu-id="527f5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="527f5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





