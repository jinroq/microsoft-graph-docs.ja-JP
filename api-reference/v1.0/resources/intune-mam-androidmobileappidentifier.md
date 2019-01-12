---
title: androidMobileAppIdentifier リソースの種類
description: Android アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6a940acc726467634df3a64dc686824350abf98f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915068"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="a205e-103">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a205e-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="a205e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a205e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a205e-105">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="a205e-105">The identifier for an Android app.</span></span>

<span data-ttu-id="a205e-106">[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a205e-106">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a205e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a205e-107">Properties</span></span>
|<span data-ttu-id="a205e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a205e-108">Property</span></span>|<span data-ttu-id="a205e-109">種類</span><span class="sxs-lookup"><span data-stu-id="a205e-109">Type</span></span>|<span data-ttu-id="a205e-110">説明</span><span class="sxs-lookup"><span data-stu-id="a205e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a205e-111">packageId</span><span class="sxs-lookup"><span data-stu-id="a205e-111">packageId</span></span>|<span data-ttu-id="a205e-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a205e-112">String</span></span>|<span data-ttu-id="a205e-113">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="a205e-113">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a205e-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a205e-114">Relationships</span></span>
<span data-ttu-id="a205e-115">なし</span><span class="sxs-lookup"><span data-stu-id="a205e-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a205e-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a205e-116">JSON Representation</span></span>
<span data-ttu-id="a205e-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a205e-117">Here is a JSON representation of the resource.</span></span>
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



