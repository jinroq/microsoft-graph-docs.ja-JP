---
title: iosHomeScreenPage リソースの種類
description: ホーム画面上のアプリとフォルダーが含まれるページ
author: tfitzmac
ms.openlocfilehash: cd7a2ee863c02aa6484889aa20003a94e525514d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325558"
---
# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="5971a-103">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5971a-103">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="5971a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5971a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5971a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5971a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5971a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5971a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5971a-107">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="5971a-107">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="5971a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5971a-108">Properties</span></span>
|<span data-ttu-id="5971a-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5971a-109">Property</span></span>|<span data-ttu-id="5971a-110">種類</span><span class="sxs-lookup"><span data-stu-id="5971a-110">Type</span></span>|<span data-ttu-id="5971a-111">説明</span><span class="sxs-lookup"><span data-stu-id="5971a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5971a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5971a-112">displayName</span></span>|<span data-ttu-id="5971a-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5971a-113">String</span></span>|<span data-ttu-id="5971a-114">ページの名前</span><span class="sxs-lookup"><span data-stu-id="5971a-114">Name of the page</span></span>|
|<span data-ttu-id="5971a-115">アイコン</span><span class="sxs-lookup"><span data-stu-id="5971a-115">icons</span></span>|<span data-ttu-id="5971a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5971a-116">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="5971a-117">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="5971a-117">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="5971a-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="5971a-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5971a-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5971a-119">Relationships</span></span>
<span data-ttu-id="5971a-120">なし</span><span class="sxs-lookup"><span data-stu-id="5971a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5971a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5971a-121">JSON Representation</span></span>
<span data-ttu-id="5971a-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5971a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```




