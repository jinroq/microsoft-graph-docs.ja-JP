---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8106475817a333838a9f7e6a591f15ddd2ce111d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563988"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="72cce-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="72cce-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="72cce-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72cce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72cce-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="72cce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72cce-106">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="72cce-106">The identifier for an Android app.</span></span>


<span data-ttu-id="72cce-107">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="72cce-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72cce-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72cce-108">Properties</span></span>
|<span data-ttu-id="72cce-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72cce-109">Property</span></span>|<span data-ttu-id="72cce-110">型</span><span class="sxs-lookup"><span data-stu-id="72cce-110">Type</span></span>|<span data-ttu-id="72cce-111">説明</span><span class="sxs-lookup"><span data-stu-id="72cce-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72cce-112">packageId</span><span class="sxs-lookup"><span data-stu-id="72cce-112">packageId</span></span>|<span data-ttu-id="72cce-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="72cce-113">String</span></span>|<span data-ttu-id="72cce-114">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="72cce-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72cce-115">関係</span><span class="sxs-lookup"><span data-stu-id="72cce-115">Relationships</span></span>
<span data-ttu-id="72cce-116">なし</span><span class="sxs-lookup"><span data-stu-id="72cce-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72cce-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="72cce-117">JSON Representation</span></span>
<span data-ttu-id="72cce-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="72cce-118">Here is a JSON representation of the resource.</span></span>
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





