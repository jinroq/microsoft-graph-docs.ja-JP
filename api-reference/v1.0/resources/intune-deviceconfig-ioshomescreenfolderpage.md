---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76a8237442e0e807e0a1383c8032cf4e6361516e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028211"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="cc5aa-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc5aa-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="cc5aa-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cc5aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc5aa-105">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="cc5aa-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="cc5aa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc5aa-106">Properties</span></span>
|<span data-ttu-id="cc5aa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc5aa-107">Property</span></span>|<span data-ttu-id="cc5aa-108">型</span><span class="sxs-lookup"><span data-stu-id="cc5aa-108">Type</span></span>|<span data-ttu-id="cc5aa-109">説明</span><span class="sxs-lookup"><span data-stu-id="cc5aa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc5aa-110">displayName</span><span class="sxs-lookup"><span data-stu-id="cc5aa-110">displayName</span></span>|<span data-ttu-id="cc5aa-111">String</span><span class="sxs-lookup"><span data-stu-id="cc5aa-111">String</span></span>|<span data-ttu-id="cc5aa-112">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="cc5aa-112">Name of the folder page</span></span>|
|<span data-ttu-id="cc5aa-113">apps</span><span class="sxs-lookup"><span data-stu-id="cc5aa-113">apps</span></span>|<span data-ttu-id="cc5aa-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="cc5aa-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="cc5aa-115">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="cc5aa-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="cc5aa-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="cc5aa-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc5aa-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc5aa-117">Relationships</span></span>
<span data-ttu-id="cc5aa-118">なし</span><span class="sxs-lookup"><span data-stu-id="cc5aa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc5aa-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc5aa-119">JSON Representation</span></span>
<span data-ttu-id="cc5aa-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc5aa-120">Here is a JSON representation of the resource.</span></span>
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



