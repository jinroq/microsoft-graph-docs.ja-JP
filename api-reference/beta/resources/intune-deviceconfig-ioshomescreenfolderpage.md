---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5bcfc7f44399de72c27a631eb0d0f04ab76bd6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813861"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="7921b-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7921b-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="7921b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7921b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7921b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7921b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7921b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7921b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7921b-107">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="7921b-107">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="7921b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7921b-108">Properties</span></span>
|<span data-ttu-id="7921b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7921b-109">Property</span></span>|<span data-ttu-id="7921b-110">種類</span><span class="sxs-lookup"><span data-stu-id="7921b-110">Type</span></span>|<span data-ttu-id="7921b-111">説明</span><span class="sxs-lookup"><span data-stu-id="7921b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7921b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7921b-112">displayName</span></span>|<span data-ttu-id="7921b-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7921b-113">String</span></span>|<span data-ttu-id="7921b-114">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="7921b-114">Name of the folder page</span></span>|
|<span data-ttu-id="7921b-115">apps</span><span class="sxs-lookup"><span data-stu-id="7921b-115">apps</span></span>|<span data-ttu-id="7921b-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7921b-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="7921b-117">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="7921b-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="7921b-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7921b-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7921b-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7921b-119">Relationships</span></span>
<span data-ttu-id="7921b-120">なし</span><span class="sxs-lookup"><span data-stu-id="7921b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7921b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7921b-121">JSON Representation</span></span>
<span data-ttu-id="7921b-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7921b-122">Here is a JSON representation of the resource.</span></span>
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





