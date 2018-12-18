---
title: iosBookmark リソースの種類
description: iOS の URL のブックマーク
author: tfitzmac
ms.openlocfilehash: e1577537e57365b2452e956e010f6c3f918bd743
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308401"
---
# <a name="iosbookmark-resource-type"></a><span data-ttu-id="f697b-103">iosBookmark リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f697b-103">iosBookmark resource type</span></span>

> <span data-ttu-id="f697b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f697b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f697b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f697b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f697b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f697b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f697b-107">iOS の URL のブックマーク</span><span class="sxs-lookup"><span data-stu-id="f697b-107">iOS URL bookmark</span></span>
## <a name="properties"></a><span data-ttu-id="f697b-108">Properties</span><span class="sxs-lookup"><span data-stu-id="f697b-108">Properties</span></span>
|<span data-ttu-id="f697b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f697b-109">Property</span></span>|<span data-ttu-id="f697b-110">種類</span><span class="sxs-lookup"><span data-stu-id="f697b-110">Type</span></span>|<span data-ttu-id="f697b-111">説明</span><span class="sxs-lookup"><span data-stu-id="f697b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f697b-112">url</span><span class="sxs-lookup"><span data-stu-id="f697b-112">url</span></span>|<span data-ttu-id="f697b-113">String</span><span class="sxs-lookup"><span data-stu-id="f697b-113">String</span></span>|<span data-ttu-id="f697b-114">URL のアクセスを許可</span><span class="sxs-lookup"><span data-stu-id="f697b-114">URL allowed to access</span></span>|
|<span data-ttu-id="f697b-115">bookmarkFolder</span><span class="sxs-lookup"><span data-stu-id="f697b-115">bookmarkFolder</span></span>|<span data-ttu-id="f697b-116">String</span><span class="sxs-lookup"><span data-stu-id="f697b-116">String</span></span>|<span data-ttu-id="f697b-117">フォルダーには、Safari でブックマークを追加します。</span><span class="sxs-lookup"><span data-stu-id="f697b-117">The folder into which the bookmark should be added in Safari</span></span>|
|<span data-ttu-id="f697b-118">displayName</span><span class="sxs-lookup"><span data-stu-id="f697b-118">displayName</span></span>|<span data-ttu-id="f697b-119">String</span><span class="sxs-lookup"><span data-stu-id="f697b-119">String</span></span>|<span data-ttu-id="f697b-120">ブックマークの表示名</span><span class="sxs-lookup"><span data-stu-id="f697b-120">The display name of the bookmark</span></span>|

## <a name="relationships"></a><span data-ttu-id="f697b-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f697b-121">Relationships</span></span>
<span data-ttu-id="f697b-122">なし</span><span class="sxs-lookup"><span data-stu-id="f697b-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f697b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f697b-123">JSON Representation</span></span>
<span data-ttu-id="f697b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f697b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```





