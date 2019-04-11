---
title: loggedOnUser リソースの種類
description: ログオンユーザー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2b92d8504ba4854109efa30d0637bca1ea35d7b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799462"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="b543e-103">loggedOnUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b543e-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="b543e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b543e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b543e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b543e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b543e-106">ログオンユーザー</span><span class="sxs-lookup"><span data-stu-id="b543e-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="b543e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b543e-107">Properties</span></span>
|<span data-ttu-id="b543e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b543e-108">Property</span></span>|<span data-ttu-id="b543e-109">型</span><span class="sxs-lookup"><span data-stu-id="b543e-109">Type</span></span>|<span data-ttu-id="b543e-110">説明</span><span class="sxs-lookup"><span data-stu-id="b543e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b543e-111">userId</span><span class="sxs-lookup"><span data-stu-id="b543e-111">userId</span></span>|<span data-ttu-id="b543e-112">String</span><span class="sxs-lookup"><span data-stu-id="b543e-112">String</span></span>|<span data-ttu-id="b543e-113">ユーザー ID</span><span class="sxs-lookup"><span data-stu-id="b543e-113">User id</span></span>|
|<span data-ttu-id="b543e-114">lastlogondatetime</span><span class="sxs-lookup"><span data-stu-id="b543e-114">lastLogOnDateTime</span></span>|<span data-ttu-id="b543e-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b543e-115">DateTimeOffset</span></span>|<span data-ttu-id="b543e-116">ユーザーがログオンした日時</span><span class="sxs-lookup"><span data-stu-id="b543e-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="b543e-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b543e-117">Relationships</span></span>
<span data-ttu-id="b543e-118">なし</span><span class="sxs-lookup"><span data-stu-id="b543e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b543e-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b543e-119">JSON Representation</span></span>
<span data-ttu-id="b543e-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b543e-120">Here is a JSON representation of the resource.</span></span>
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





