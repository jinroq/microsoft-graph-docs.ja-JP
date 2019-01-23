---
title: IosLobAppProvisioningConfigurationAssignment を更新します。
description: IosLobAppProvisioningConfigurationAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f80f07feb9027054b5b88f1fa4fdcf868e0b3f84
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397618"
---
# <a name="update-ioslobappprovisioningconfigurationassignment"></a><span data-ttu-id="b66fb-103">IosLobAppProvisioningConfigurationAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="b66fb-103">Update iosLobAppProvisioningConfigurationAssignment</span></span>

> <span data-ttu-id="b66fb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b66fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b66fb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b66fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b66fb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b66fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b66fb-107">[IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b66fb-107">Update the properties of a [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b66fb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b66fb-108">Prerequisites</span></span>
<span data-ttu-id="b66fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b66fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b66fb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b66fb-111">Permission type</span></span>|<span data-ttu-id="b66fb-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b66fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b66fb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b66fb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b66fb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b66fb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b66fb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b66fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b66fb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b66fb-116">Not supported.</span></span>|
|<span data-ttu-id="b66fb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b66fb-117">Application</span></span>|<span data-ttu-id="b66fb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b66fb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b66fb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b66fb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b66fb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b66fb-120">Request headers</span></span>
|<span data-ttu-id="b66fb-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b66fb-121">Header</span></span>|<span data-ttu-id="b66fb-122">値</span><span class="sxs-lookup"><span data-stu-id="b66fb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b66fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b66fb-123">Authorization</span></span>|<span data-ttu-id="b66fb-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b66fb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b66fb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b66fb-125">Accept</span></span>|<span data-ttu-id="b66fb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b66fb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b66fb-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b66fb-127">Request body</span></span>
<span data-ttu-id="b66fb-128">要求の本文に[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b66fb-128">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object.</span></span>

<span data-ttu-id="b66fb-129">[IosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="b66fb-129">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md).</span></span>

|<span data-ttu-id="b66fb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b66fb-130">Property</span></span>|<span data-ttu-id="b66fb-131">型</span><span class="sxs-lookup"><span data-stu-id="b66fb-131">Type</span></span>|<span data-ttu-id="b66fb-132">説明</span><span class="sxs-lookup"><span data-stu-id="b66fb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b66fb-133">id</span><span class="sxs-lookup"><span data-stu-id="b66fb-133">id</span></span>|<span data-ttu-id="b66fb-134">String</span><span class="sxs-lookup"><span data-stu-id="b66fb-134">String</span></span>|<span data-ttu-id="b66fb-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b66fb-135">Key of the entity.</span></span>|
|<span data-ttu-id="b66fb-136">target</span><span class="sxs-lookup"><span data-stu-id="b66fb-136">target</span></span>|[<span data-ttu-id="b66fb-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b66fb-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b66fb-138">管理者によって定義された、ターゲット グループの割り当て。</span><span class="sxs-lookup"><span data-stu-id="b66fb-138">The target group assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="b66fb-139">応答</span><span class="sxs-lookup"><span data-stu-id="b66fb-139">Response</span></span>
<span data-ttu-id="b66fb-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b66fb-140">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfigurationAssignment](../resources/intune-apps-ioslobappprovisioningconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b66fb-141">例</span><span class="sxs-lookup"><span data-stu-id="b66fb-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b66fb-142">要求</span><span class="sxs-lookup"><span data-stu-id="b66fb-142">Request</span></span>
<span data-ttu-id="b66fb-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b66fb-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/assignments/{iosLobAppProvisioningConfigurationAssignmentId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="b66fb-144">応答</span><span class="sxs-lookup"><span data-stu-id="b66fb-144">Response</span></span>
<span data-ttu-id="b66fb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b66fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "eac7008e-008e-eac7-8e00-c7ea8e00c7ea",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




