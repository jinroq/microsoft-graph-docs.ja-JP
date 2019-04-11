---
title: manageddevicereportedapp リソースの種類
description: レポート用のアプリケーションデータ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b243cbc5c3c06de6af3e2e0f1263b589edf86f48
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801170"
---
# <a name="manageddevicereportedapp-resource-type"></a><span data-ttu-id="61ee1-103">manageddevicereportedapp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="61ee1-103">managedDeviceReportedApp resource type</span></span>

> <span data-ttu-id="61ee1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61ee1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61ee1-106">レポート用のアプリケーションデータ</span><span class="sxs-lookup"><span data-stu-id="61ee1-106">Application data for reporting</span></span>

## <a name="properties"></a><span data-ttu-id="61ee1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61ee1-107">Properties</span></span>
|<span data-ttu-id="61ee1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61ee1-108">Property</span></span>|<span data-ttu-id="61ee1-109">型</span><span class="sxs-lookup"><span data-stu-id="61ee1-109">Type</span></span>|<span data-ttu-id="61ee1-110">説明</span><span class="sxs-lookup"><span data-stu-id="61ee1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61ee1-111">appId</span><span class="sxs-lookup"><span data-stu-id="61ee1-111">appId</span></span>|<span data-ttu-id="61ee1-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="61ee1-112">String</span></span>|<span data-ttu-id="61ee1-113">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="61ee1-113">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="61ee1-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="61ee1-114">Relationships</span></span>
<span data-ttu-id="61ee1-115">なし</span><span class="sxs-lookup"><span data-stu-id="61ee1-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61ee1-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="61ee1-116">JSON Representation</span></span>
<span data-ttu-id="61ee1-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="61ee1-117">Here is a JSON representation of the resource.</span></span>
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





