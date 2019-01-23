---
title: loggedOnUser リソースの種類
description: ログオン中のユーザー
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ac0ca08c6d324836e4bb9dd9951fdfe742b8b5f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395196"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="b2dfa-103">loggedOnUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2dfa-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="b2dfa-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b2dfa-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b2dfa-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2dfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2dfa-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b2dfa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2dfa-107">ログオン中のユーザー</span><span class="sxs-lookup"><span data-stu-id="b2dfa-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="b2dfa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2dfa-108">Properties</span></span>
|<span data-ttu-id="b2dfa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2dfa-109">Property</span></span>|<span data-ttu-id="b2dfa-110">型</span><span class="sxs-lookup"><span data-stu-id="b2dfa-110">Type</span></span>|<span data-ttu-id="b2dfa-111">説明</span><span class="sxs-lookup"><span data-stu-id="b2dfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2dfa-112">userId</span><span class="sxs-lookup"><span data-stu-id="b2dfa-112">userId</span></span>|<span data-ttu-id="b2dfa-113">String</span><span class="sxs-lookup"><span data-stu-id="b2dfa-113">String</span></span>|<span data-ttu-id="b2dfa-114">ユーザー id</span><span class="sxs-lookup"><span data-stu-id="b2dfa-114">User id</span></span>|
|<span data-ttu-id="b2dfa-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="b2dfa-115">lastLogOnDateTime</span></span>|<span data-ttu-id="b2dfa-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2dfa-116">DateTimeOffset</span></span>|<span data-ttu-id="b2dfa-117">ユーザーのログオン時の日付します。</span><span class="sxs-lookup"><span data-stu-id="b2dfa-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2dfa-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2dfa-118">Relationships</span></span>
<span data-ttu-id="b2dfa-119">なし</span><span class="sxs-lookup"><span data-stu-id="b2dfa-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2dfa-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2dfa-120">JSON Representation</span></span>
<span data-ttu-id="b2dfa-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2dfa-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




