---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: tfitzmac
ms.openlocfilehash: 983337c4376bb6212607630f96008a2c8a36b22b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306693"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="00b45-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="00b45-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="00b45-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00b45-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00b45-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00b45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00b45-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="00b45-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00b45-107">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="00b45-107">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="00b45-108">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="00b45-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="00b45-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00b45-109">Properties</span></span>
|<span data-ttu-id="00b45-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00b45-110">Property</span></span>|<span data-ttu-id="00b45-111">種類</span><span class="sxs-lookup"><span data-stu-id="00b45-111">Type</span></span>|<span data-ttu-id="00b45-112">説明</span><span class="sxs-lookup"><span data-stu-id="00b45-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00b45-113">displayName</span><span class="sxs-lookup"><span data-stu-id="00b45-113">displayName</span></span>|<span data-ttu-id="00b45-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="00b45-114">String</span></span>|<span data-ttu-id="00b45-115">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="00b45-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="00b45-116">pages</span><span class="sxs-lookup"><span data-stu-id="00b45-116">pages</span></span>|<span data-ttu-id="00b45-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="00b45-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="00b45-118">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="00b45-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="00b45-119">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="00b45-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00b45-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="00b45-120">Relationships</span></span>
<span data-ttu-id="00b45-121">なし</span><span class="sxs-lookup"><span data-stu-id="00b45-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00b45-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="00b45-122">JSON Representation</span></span>
<span data-ttu-id="00b45-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="00b45-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```




