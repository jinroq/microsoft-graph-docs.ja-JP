---
title: manageddevicereportedapp リソースの種類
description: レポート用のアプリケーションデータ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3e1cd99974259835859cf8a2fc6a9f197c09d4d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166270"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="3986a-103">manageddevicereportedapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3986a-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="3986a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3986a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3986a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3986a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3986a-106">レポート用のアプリケーションデータ</span><span class="sxs-lookup"><span data-stu-id="3986a-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="3986a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3986a-107">Properties</span></span>
|<span data-ttu-id="3986a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3986a-108">Property</span></span>|<span data-ttu-id="3986a-109">型</span><span class="sxs-lookup"><span data-stu-id="3986a-109">Type</span></span>|<span data-ttu-id="3986a-110">説明</span><span class="sxs-lookup"><span data-stu-id="3986a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3986a-111">appId</span><span class="sxs-lookup"><span data-stu-id="3986a-111">appId</span></span>|<span data-ttu-id="3986a-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3986a-112">String</span></span>|<span data-ttu-id="3986a-113">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="3986a-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="3986a-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3986a-114">Relationships</span></span>
<span data-ttu-id="3986a-115">なし</span><span class="sxs-lookup"><span data-stu-id="3986a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3986a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3986a-116">JSON Representation</span></span>
<span data-ttu-id="3986a-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3986a-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```




