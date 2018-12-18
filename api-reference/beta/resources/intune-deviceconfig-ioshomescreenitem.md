---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: tfitzmac
ms.openlocfilehash: 6a8d71e01ca8f2c284bcc3eddd7eb39b87c025d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328190"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="5ac19-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ac19-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="5ac19-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5ac19-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ac19-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ac19-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ac19-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ac19-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ac19-107">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="5ac19-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="5ac19-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ac19-108">Properties</span></span>
|<span data-ttu-id="5ac19-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ac19-109">Property</span></span>|<span data-ttu-id="5ac19-110">種類</span><span class="sxs-lookup"><span data-stu-id="5ac19-110">Type</span></span>|<span data-ttu-id="5ac19-111">説明</span><span class="sxs-lookup"><span data-stu-id="5ac19-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ac19-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5ac19-112">displayName</span></span>|<span data-ttu-id="5ac19-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5ac19-113">String</span></span>|<span data-ttu-id="5ac19-114">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="5ac19-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ac19-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5ac19-115">Relationships</span></span>
<span data-ttu-id="5ac19-116">なし</span><span class="sxs-lookup"><span data-stu-id="5ac19-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5ac19-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ac19-117">JSON Representation</span></span>
<span data-ttu-id="5ac19-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ac19-118">Here is a JSON representation of the resource.</span></span>
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





