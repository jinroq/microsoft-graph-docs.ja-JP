---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
author: tfitzmac
ms.openlocfilehash: 147504fc356f3a4092b2ffd1c7d03275ff7dea31
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353642"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="b2b57-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2b57-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="b2b57-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2b57-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2b57-105">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="b2b57-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="b2b57-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2b57-106">Properties</span></span>
|<span data-ttu-id="b2b57-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2b57-107">Property</span></span>|<span data-ttu-id="b2b57-108">種類</span><span class="sxs-lookup"><span data-stu-id="b2b57-108">Type</span></span>|<span data-ttu-id="b2b57-109">説明</span><span class="sxs-lookup"><span data-stu-id="b2b57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2b57-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b2b57-110">displayName</span></span>|<span data-ttu-id="b2b57-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b2b57-111">String</span></span>|<span data-ttu-id="b2b57-112">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="b2b57-112">Name of the folder page</span></span>|
|<span data-ttu-id="b2b57-113">apps</span><span class="sxs-lookup"><span data-stu-id="b2b57-113">apps</span></span>|<span data-ttu-id="b2b57-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b2b57-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="b2b57-115">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="b2b57-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="b2b57-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b2b57-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2b57-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2b57-117">Relationships</span></span>
<span data-ttu-id="b2b57-118">なし</span><span class="sxs-lookup"><span data-stu-id="b2b57-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2b57-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2b57-119">JSON Representation</span></span>
<span data-ttu-id="b2b57-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2b57-120">Here is a JSON representation of the resource.</span></span>
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



