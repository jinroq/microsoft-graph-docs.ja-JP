---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 26c258dbf0091b44d2f7eea8fdf4066a5c8e6729
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969773"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="7e8ae-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e8ae-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="7e8ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7e8ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e8ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e8ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e8ae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e8ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e8ae-107">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="7e8ae-107">The identifier for an Android app.</span></span>

<span data-ttu-id="7e8ae-108">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7e8ae-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e8ae-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e8ae-109">Properties</span></span>
|<span data-ttu-id="7e8ae-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e8ae-110">Property</span></span>|<span data-ttu-id="7e8ae-111">種類</span><span class="sxs-lookup"><span data-stu-id="7e8ae-111">Type</span></span>|<span data-ttu-id="7e8ae-112">説明</span><span class="sxs-lookup"><span data-stu-id="7e8ae-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e8ae-113">packageId</span><span class="sxs-lookup"><span data-stu-id="7e8ae-113">packageId</span></span>|<span data-ttu-id="7e8ae-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7e8ae-114">String</span></span>|<span data-ttu-id="7e8ae-115">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="7e8ae-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e8ae-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e8ae-116">Relationships</span></span>
<span data-ttu-id="7e8ae-117">なし</span><span class="sxs-lookup"><span data-stu-id="7e8ae-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7e8ae-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e8ae-118">JSON Representation</span></span>
<span data-ttu-id="7e8ae-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e8ae-119">Here is a JSON representation of the resource.</span></span>
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





