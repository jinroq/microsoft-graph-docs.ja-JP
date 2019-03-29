---
title: mobileAppProvisioningConfigGroupAssignment の更新
description: mobileAppProvisioningConfigGroupAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3574b569dca591e1bebb70558ef06a1d43f52ca
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963983"
---
# <a name="update-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="3ae2b-103">mobileAppProvisioningConfigGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="3ae2b-103">Update mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="3ae2b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ae2b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ae2b-106">[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-106">Update the properties of a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ae2b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3ae2b-107">Prerequisites</span></span>
<span data-ttu-id="3ae2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ae2b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ae2b-110">Permission type</span></span>|<span data-ttu-id="3ae2b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ae2b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ae2b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ae2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3ae2b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ae2b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ae2b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ae2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ae2b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-115">Not supported.</span></span>|
|<span data-ttu-id="3ae2b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ae2b-116">Application</span></span>|<span data-ttu-id="3ae2b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ae2b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ae2b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="3ae2b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ae2b-119">Request headers</span></span>
|<span data-ttu-id="3ae2b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ae2b-120">Header</span></span>|<span data-ttu-id="3ae2b-121">値</span><span class="sxs-lookup"><span data-stu-id="3ae2b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ae2b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ae2b-122">Authorization</span></span>|<span data-ttu-id="3ae2b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ae2b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3ae2b-124">Accept</span></span>|<span data-ttu-id="3ae2b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3ae2b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ae2b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ae2b-126">Request body</span></span>
<span data-ttu-id="3ae2b-127">要求本文で、 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-127">In the request body, supply a JSON representation for the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object.</span></span>

<span data-ttu-id="3ae2b-128">次の表に、 [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-128">The following table shows the properties that are required when you create the [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

|<span data-ttu-id="3ae2b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ae2b-129">Property</span></span>|<span data-ttu-id="3ae2b-130">型</span><span class="sxs-lookup"><span data-stu-id="3ae2b-130">Type</span></span>|<span data-ttu-id="3ae2b-131">説明</span><span class="sxs-lookup"><span data-stu-id="3ae2b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ae2b-132">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="3ae2b-132">targetGroupId</span></span>|<span data-ttu-id="3ae2b-133">String</span><span class="sxs-lookup"><span data-stu-id="3ae2b-133">String</span></span>|<span data-ttu-id="3ae2b-134">アプリのプロビジョニング構成を対象とする AAD グループの ID。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-134">The ID of the AAD group in which the app provisioning configuration is being targeted.</span></span>|
|<span data-ttu-id="3ae2b-135">id</span><span class="sxs-lookup"><span data-stu-id="3ae2b-135">id</span></span>|<span data-ttu-id="3ae2b-136">String</span><span class="sxs-lookup"><span data-stu-id="3ae2b-136">String</span></span>|<span data-ttu-id="3ae2b-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-137">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="3ae2b-138">応答</span><span class="sxs-lookup"><span data-stu-id="3ae2b-138">Response</span></span>
<span data-ttu-id="3ae2b-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-139">If successful, this method returns a `200 OK` response code and an updated [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ae2b-140">例</span><span class="sxs-lookup"><span data-stu-id="3ae2b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ae2b-141">要求</span><span class="sxs-lookup"><span data-stu-id="3ae2b-141">Request</span></span>
<span data-ttu-id="3ae2b-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
Content-type: application/json
Content-length: 129

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="3ae2b-143">応答</span><span class="sxs-lookup"><span data-stu-id="3ae2b-143">Response</span></span>
<span data-ttu-id="3ae2b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3ae2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 178

{
  "@odata.type": "#microsoft.graph.mobileAppProvisioningConfigGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "id": "fad873e3-73e3-fad8-e373-d8fae373d8fa"
}
```




