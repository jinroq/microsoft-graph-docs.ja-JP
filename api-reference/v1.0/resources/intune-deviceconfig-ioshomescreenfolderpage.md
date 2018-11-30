---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
ms.openlocfilehash: ce8332435f55ac4941c80ed60fdbf17f417e1008
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020221"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="9a32b-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9a32b-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="9a32b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a32b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9a32b-105">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="9a32b-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="9a32b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a32b-106">Properties</span></span>
|<span data-ttu-id="9a32b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9a32b-107">Property</span></span>|<span data-ttu-id="9a32b-108">型</span><span class="sxs-lookup"><span data-stu-id="9a32b-108">Type</span></span>|<span data-ttu-id="9a32b-109">説明</span><span class="sxs-lookup"><span data-stu-id="9a32b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a32b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9a32b-110">displayName</span></span>|<span data-ttu-id="9a32b-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9a32b-111">String</span></span>|<span data-ttu-id="9a32b-112">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="9a32b-112">Name of the folder page</span></span>|
|<span data-ttu-id="9a32b-113">apps</span><span class="sxs-lookup"><span data-stu-id="9a32b-113">apps</span></span>|<span data-ttu-id="9a32b-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9a32b-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="9a32b-115">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="9a32b-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="9a32b-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9a32b-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a32b-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9a32b-117">Relationships</span></span>
<span data-ttu-id="9a32b-118">なし</span><span class="sxs-lookup"><span data-stu-id="9a32b-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9a32b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9a32b-119">JSON Representation</span></span>
<span data-ttu-id="9a32b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9a32b-120">Here is a JSON representation of the resource.</span></span>
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



