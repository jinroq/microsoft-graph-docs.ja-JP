---
title: 組織を更新する
description: organization オブジェクトのプロパティを更新します。
ms.openlocfilehash: 32e9cf3cccecf0a763d20b201040d79d4442cdfe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074467"
---
# <a name="update-organization"></a><span data-ttu-id="c2a2c-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="c2a2c-103">Update organization</span></span>

> <span data-ttu-id="c2a2c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2a2c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2a2c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2a2c-107">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2a2c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c2a2c-108">Prerequisites</span></span>
<span data-ttu-id="c2a2c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2a2c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2a2c-111">Permission type</span></span>|<span data-ttu-id="c2a2c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2a2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2a2c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2a2c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2a2c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2a2c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c2a2c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2a2c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2a2c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-116">Not supported.</span></span>|
|<span data-ttu-id="c2a2c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2a2c-117">Application</span></span>|<span data-ttu-id="c2a2c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2a2c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2a2c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="c2a2c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2a2c-120">Request headers</span></span>
|<span data-ttu-id="c2a2c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2a2c-121">Header</span></span>|<span data-ttu-id="c2a2c-122">値</span><span class="sxs-lookup"><span data-stu-id="c2a2c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2a2c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2a2c-123">Authorization</span></span>|<span data-ttu-id="c2a2c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2a2c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2a2c-125">Accept</span></span>|<span data-ttu-id="c2a2c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2a2c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2a2c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2a2c-127">Request body</span></span>
<span data-ttu-id="c2a2c-128">要求本文で、[organization](../resources/intune-onboarding-organization.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="c2a2c-129">次の表に、[organization](../resources/intune-onboarding-organization.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="c2a2c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2a2c-130">Property</span></span>|<span data-ttu-id="c2a2c-131">型</span><span class="sxs-lookup"><span data-stu-id="c2a2c-131">Type</span></span>|<span data-ttu-id="c2a2c-132">説明</span><span class="sxs-lookup"><span data-stu-id="c2a2c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2a2c-133">id</span><span class="sxs-lookup"><span data-stu-id="c2a2c-133">id</span></span>|<span data-ttu-id="c2a2c-134">String</span><span class="sxs-lookup"><span data-stu-id="c2a2c-134">String</span></span>|<span data-ttu-id="c2a2c-135">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-135">The GUID for the object.</span></span>|
|<span data-ttu-id="c2a2c-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="c2a2c-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="c2a2c-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="c2a2c-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="c2a2c-138">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-138">Mobile device management authority.</span></span> <span data-ttu-id="c2a2c-139">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="c2a2c-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c2a2c-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="c2a2c-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="c2a2c-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="c2a2c-142">コネクタ証明書の設定です。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="c2a2c-143">応答</span><span class="sxs-lookup"><span data-stu-id="c2a2c-143">Response</span></span>
<span data-ttu-id="c2a2c-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/intune-onboarding-organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2a2c-145">例</span><span class="sxs-lookup"><span data-stu-id="c2a2c-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2a2c-146">要求</span><span class="sxs-lookup"><span data-stu-id="c2a2c-146">Request</span></span>
<span data-ttu-id="c2a2c-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}
Content-type: application/json
Content-length: 441

{
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

### <a name="response"></a><span data-ttu-id="c2a2c-148">応答</span><span class="sxs-lookup"><span data-stu-id="c2a2c-148">Response</span></span>
<span data-ttu-id="c2a2c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2a2c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




