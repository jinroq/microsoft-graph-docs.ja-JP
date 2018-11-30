---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
ms.openlocfilehash: 705849569dd91d339633e52187d16dfdd25b5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071786"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="c5aab-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5aab-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="c5aab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c5aab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5aab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5aab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5aab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5aab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5aab-107">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="c5aab-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="c5aab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5aab-108">Properties</span></span>
|<span data-ttu-id="c5aab-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5aab-109">Property</span></span>|<span data-ttu-id="c5aab-110">型</span><span class="sxs-lookup"><span data-stu-id="c5aab-110">Type</span></span>|<span data-ttu-id="c5aab-111">説明</span><span class="sxs-lookup"><span data-stu-id="c5aab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5aab-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c5aab-112">displayName</span></span>|<span data-ttu-id="c5aab-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c5aab-113">String</span></span>|<span data-ttu-id="c5aab-114">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="c5aab-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5aab-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c5aab-115">Relationships</span></span>
<span data-ttu-id="c5aab-116">なし</span><span class="sxs-lookup"><span data-stu-id="c5aab-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c5aab-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5aab-117">JSON Representation</span></span>
<span data-ttu-id="c5aab-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c5aab-118">Here is a JSON representation of the resource.</span></span>
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





