---
title: 組織を更新する
description: organization オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1f1a2e48e882cf6e314f3aa58a2c7bab99b2832
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157758"
---
# <a name="update-organization"></a><span data-ttu-id="9186d-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="9186d-103">Update organization</span></span>

> <span data-ttu-id="9186d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9186d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9186d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9186d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9186d-106">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9186d-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9186d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9186d-107">Prerequisites</span></span>
<span data-ttu-id="9186d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9186d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9186d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9186d-110">Permission type</span></span>|<span data-ttu-id="9186d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9186d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9186d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9186d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9186d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9186d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9186d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9186d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9186d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9186d-115">Not supported.</span></span>|
|<span data-ttu-id="9186d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9186d-116">Application</span></span>|<span data-ttu-id="9186d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9186d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9186d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9186d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="9186d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9186d-119">Request headers</span></span>
|<span data-ttu-id="9186d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9186d-120">Header</span></span>|<span data-ttu-id="9186d-121">値</span><span class="sxs-lookup"><span data-stu-id="9186d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9186d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9186d-122">Authorization</span></span>|<span data-ttu-id="9186d-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9186d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9186d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9186d-124">Accept</span></span>|<span data-ttu-id="9186d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9186d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9186d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9186d-126">Request body</span></span>
<span data-ttu-id="9186d-127">要求本文で、[organization](../resources/intune-onboarding-organization.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9186d-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="9186d-128">次の表に、[organization](../resources/intune-onboarding-organization.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9186d-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="9186d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9186d-129">Property</span></span>|<span data-ttu-id="9186d-130">型</span><span class="sxs-lookup"><span data-stu-id="9186d-130">Type</span></span>|<span data-ttu-id="9186d-131">説明</span><span class="sxs-lookup"><span data-stu-id="9186d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9186d-132">id</span><span class="sxs-lookup"><span data-stu-id="9186d-132">id</span></span>|<span data-ttu-id="9186d-133">String</span><span class="sxs-lookup"><span data-stu-id="9186d-133">String</span></span>|<span data-ttu-id="9186d-134">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="9186d-134">The GUID for the object.</span></span>|
|<span data-ttu-id="9186d-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="9186d-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="9186d-136">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="9186d-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="9186d-137">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="9186d-137">Mobile device management authority.</span></span> <span data-ttu-id="9186d-138">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="9186d-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="9186d-139">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="9186d-139">certificateConnectorSetting</span></span>|[<span data-ttu-id="9186d-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="9186d-140">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="9186d-141">証明書コネクタの設定。</span><span class="sxs-lookup"><span data-stu-id="9186d-141">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="9186d-142">応答</span><span class="sxs-lookup"><span data-stu-id="9186d-142">Response</span></span>
<span data-ttu-id="9186d-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/intune-onboarding-organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9186d-143">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9186d-144">例</span><span class="sxs-lookup"><span data-stu-id="9186d-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="9186d-145">要求</span><span class="sxs-lookup"><span data-stu-id="9186d-145">Request</span></span>
<span data-ttu-id="9186d-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9186d-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```

### <a name="response"></a><span data-ttu-id="9186d-147">応答</span><span class="sxs-lookup"><span data-stu-id="9186d-147">Response</span></span>
<span data-ttu-id="9186d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9186d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 541

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 6,
    "certExpiryTime": "2017-01-01T00:00:03.9979674-08:00",
    "enrollmentError": "Enrollment Error value",
    "lastConnectorConnectionTime": "2017-01-01T00:02:50.2393584-08:00",
    "connectorVersion": "Connector Version value",
    "lastUploadVersion": 1
  }
}
```




