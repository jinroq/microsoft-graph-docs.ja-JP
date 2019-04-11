---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8106475817a333838a9f7e6a591f15ddd2ce111d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805734"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="45786-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45786-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="45786-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45786-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45786-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45786-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45786-106">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="45786-106">The identifier for an Android app.</span></span>


<span data-ttu-id="45786-107">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="45786-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45786-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45786-108">Properties</span></span>
|<span data-ttu-id="45786-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45786-109">Property</span></span>|<span data-ttu-id="45786-110">型</span><span class="sxs-lookup"><span data-stu-id="45786-110">Type</span></span>|<span data-ttu-id="45786-111">説明</span><span class="sxs-lookup"><span data-stu-id="45786-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45786-112">packageId</span><span class="sxs-lookup"><span data-stu-id="45786-112">packageId</span></span>|<span data-ttu-id="45786-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="45786-113">String</span></span>|<span data-ttu-id="45786-114">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="45786-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45786-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45786-115">Relationships</span></span>
<span data-ttu-id="45786-116">なし</span><span class="sxs-lookup"><span data-stu-id="45786-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45786-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45786-117">JSON Representation</span></span>
<span data-ttu-id="45786-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45786-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```





