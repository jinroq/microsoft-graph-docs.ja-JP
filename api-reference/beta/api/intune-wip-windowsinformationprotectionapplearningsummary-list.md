---
title: windowsInformationProtectionAppLearningSummaries のリスト
description: windowsInformationProtectionAppLearningSummary オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e1b58a6264a9809bfc4d3c3034dfd22323ea2d75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979163"
---
# <a name="list-windowsinformationprotectionapplearningsummaries"></a><span data-ttu-id="0540f-103">windowsInformationProtectionAppLearningSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="0540f-103">List windowsInformationProtectionAppLearningSummaries</span></span>

> <span data-ttu-id="0540f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0540f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0540f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0540f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0540f-106">[windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0540f-106">List properties and relationships of the [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0540f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0540f-107">Prerequisites</span></span>
<span data-ttu-id="0540f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0540f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0540f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0540f-110">Permission type</span></span>|<span data-ttu-id="0540f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0540f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0540f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0540f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0540f-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0540f-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0540f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0540f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0540f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0540f-115">Not supported.</span></span>|
|<span data-ttu-id="0540f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0540f-116">Application</span></span>|<span data-ttu-id="0540f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0540f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0540f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0540f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="0540f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0540f-119">Request headers</span></span>
|<span data-ttu-id="0540f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0540f-120">Header</span></span>|<span data-ttu-id="0540f-121">値</span><span class="sxs-lookup"><span data-stu-id="0540f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0540f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0540f-122">Authorization</span></span>|<span data-ttu-id="0540f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0540f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0540f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0540f-124">Accept</span></span>|<span data-ttu-id="0540f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0540f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0540f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0540f-126">Request body</span></span>
<span data-ttu-id="0540f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0540f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0540f-128">応答</span><span class="sxs-lookup"><span data-stu-id="0540f-128">Response</span></span>
<span data-ttu-id="0540f-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0540f-129">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionAppLearningSummary](../resources/intune-wip-windowsinformationprotectionapplearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0540f-130">例</span><span class="sxs-lookup"><span data-stu-id="0540f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0540f-131">要求</span><span class="sxs-lookup"><span data-stu-id="0540f-131">Request</span></span>
<span data-ttu-id="0540f-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0540f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
```

### <a name="response"></a><span data-ttu-id="0540f-133">応答</span><span class="sxs-lookup"><span data-stu-id="0540f-133">Response</span></span>
<span data-ttu-id="0540f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0540f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
      "id": "063baf50-af50-063b-50af-3b0650af3b06",
      "applicationName": "Application Name value",
      "applicationType": "desktop",
      "deviceCount": 11
    }
  ]
}
```





