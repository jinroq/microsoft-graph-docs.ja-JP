---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38b1d898cb4bc1eacaa427ed412b536ba40cd0f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941962"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="39ab9-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39ab9-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="39ab9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39ab9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39ab9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39ab9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39ab9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39ab9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39ab9-107">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="39ab9-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="39ab9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39ab9-108">Properties</span></span>
|<span data-ttu-id="39ab9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39ab9-109">Property</span></span>|<span data-ttu-id="39ab9-110">種類</span><span class="sxs-lookup"><span data-stu-id="39ab9-110">Type</span></span>|<span data-ttu-id="39ab9-111">説明</span><span class="sxs-lookup"><span data-stu-id="39ab9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ab9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="39ab9-112">displayName</span></span>|<span data-ttu-id="39ab9-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="39ab9-113">String</span></span>|<span data-ttu-id="39ab9-114">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="39ab9-114">Name of the folder page</span></span>|
|<span data-ttu-id="39ab9-115">apps</span><span class="sxs-lookup"><span data-stu-id="39ab9-115">apps</span></span>|<span data-ttu-id="39ab9-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="39ab9-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="39ab9-117">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="39ab9-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="39ab9-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="39ab9-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ab9-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39ab9-119">Relationships</span></span>
<span data-ttu-id="39ab9-120">なし</span><span class="sxs-lookup"><span data-stu-id="39ab9-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39ab9-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39ab9-121">JSON Representation</span></span>
<span data-ttu-id="39ab9-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39ab9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```





