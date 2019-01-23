---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa9462f8fb0640584515d1c209abd03de0e6200
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424176"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="16f79-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16f79-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="16f79-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16f79-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16f79-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16f79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16f79-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16f79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16f79-107">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="16f79-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="16f79-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16f79-108">Properties</span></span>
|<span data-ttu-id="16f79-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16f79-109">Property</span></span>|<span data-ttu-id="16f79-110">型</span><span class="sxs-lookup"><span data-stu-id="16f79-110">Type</span></span>|<span data-ttu-id="16f79-111">説明</span><span class="sxs-lookup"><span data-stu-id="16f79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16f79-112">displayName</span><span class="sxs-lookup"><span data-stu-id="16f79-112">displayName</span></span>|<span data-ttu-id="16f79-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="16f79-113">String</span></span>|<span data-ttu-id="16f79-114">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="16f79-114">Name of the folder page</span></span>|
|<span data-ttu-id="16f79-115">apps</span><span class="sxs-lookup"><span data-stu-id="16f79-115">apps</span></span>|<span data-ttu-id="16f79-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="16f79-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="16f79-117">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="16f79-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="16f79-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="16f79-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16f79-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="16f79-119">Relationships</span></span>
<span data-ttu-id="16f79-120">なし</span><span class="sxs-lookup"><span data-stu-id="16f79-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16f79-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16f79-121">JSON Representation</span></span>
<span data-ttu-id="16f79-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="16f79-122">Here is a JSON representation of the resource.</span></span>
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




