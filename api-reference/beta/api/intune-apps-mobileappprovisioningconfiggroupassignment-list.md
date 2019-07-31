---
title: リスト mobileAppProvisioningConfigGroupAssignments
description: MobileAppProvisioningConfigGroupAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73438275f1b4bd2abce2c19d0dff594588361cdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960616"
---
# <a name="list-mobileappprovisioningconfiggroupassignments"></a><span data-ttu-id="4b0ea-103">リスト mobileAppProvisioningConfigGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="4b0ea-103">List mobileAppProvisioningConfigGroupAssignments</span></span>

> <span data-ttu-id="4b0ea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b0ea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b0ea-106">[MobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-106">List properties and relationships of the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b0ea-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4b0ea-107">Prerequisites</span></span>
<span data-ttu-id="4b0ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b0ea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b0ea-110">Permission type</span></span>|<span data-ttu-id="4b0ea-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b0ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b0ea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b0ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4b0ea-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4b0ea-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4b0ea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b0ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b0ea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-115">Not supported.</span></span>|
|<span data-ttu-id="4b0ea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b0ea-116">Application</span></span>|<span data-ttu-id="4b0ea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b0ea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b0ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="4b0ea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b0ea-119">Request headers</span></span>
|<span data-ttu-id="4b0ea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b0ea-120">Header</span></span>|<span data-ttu-id="4b0ea-121">値</span><span class="sxs-lookup"><span data-stu-id="4b0ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b0ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b0ea-122">Authorization</span></span>|<span data-ttu-id="4b0ea-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b0ea-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4b0ea-124">Accept</span></span>|<span data-ttu-id="4b0ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4b0ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b0ea-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b0ea-126">Request body</span></span>
<span data-ttu-id="4b0ea-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b0ea-128">応答</span><span class="sxs-lookup"><span data-stu-id="4b0ea-128">Response</span></span>
<span data-ttu-id="4b0ea-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b0ea-130">例</span><span class="sxs-lookup"><span data-stu-id="4b0ea-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b0ea-131">要求</span><span class="sxs-lookup"><span data-stu-id="4b0ea-131">Request</span></span>
<span data-ttu-id="4b0ea-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="4b0ea-133">応答</span><span class="sxs-lookup"><span data-stu-id="4b0ea-133">Response</span></span>
<span data-ttu-id="4b0ea-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b0ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
      "targetGroupId": "Target Group Id value",
      "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
    }
  ]
}
```





