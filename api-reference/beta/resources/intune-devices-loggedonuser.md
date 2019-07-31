---
title: loggedOnUser リソースの種類
description: ログオンユーザー
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a6b58667933d530f91685f6fd12a8e5f63ea831
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999781"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="ba58b-103">loggedOnUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba58b-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="ba58b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba58b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba58b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba58b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba58b-106">ログオンユーザー</span><span class="sxs-lookup"><span data-stu-id="ba58b-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="ba58b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba58b-107">Properties</span></span>
|<span data-ttu-id="ba58b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba58b-108">Property</span></span>|<span data-ttu-id="ba58b-109">型</span><span class="sxs-lookup"><span data-stu-id="ba58b-109">Type</span></span>|<span data-ttu-id="ba58b-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba58b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba58b-111">userId</span><span class="sxs-lookup"><span data-stu-id="ba58b-111">userId</span></span>|<span data-ttu-id="ba58b-112">String</span><span class="sxs-lookup"><span data-stu-id="ba58b-112">String</span></span>|<span data-ttu-id="ba58b-113">ユーザー ID</span><span class="sxs-lookup"><span data-stu-id="ba58b-113">User id</span></span>|
|<span data-ttu-id="ba58b-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="ba58b-114">lastLogOnDateTime</span></span>|<span data-ttu-id="ba58b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba58b-115">DateTimeOffset</span></span>|<span data-ttu-id="ba58b-116">ユーザーがログオンした日時</span><span class="sxs-lookup"><span data-stu-id="ba58b-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba58b-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ba58b-117">Relationships</span></span>
<span data-ttu-id="ba58b-118">なし</span><span class="sxs-lookup"><span data-stu-id="ba58b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba58b-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba58b-119">JSON Representation</span></span>
<span data-ttu-id="ba58b-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba58b-120">Here is a JSON representation of the resource.</span></span>
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





