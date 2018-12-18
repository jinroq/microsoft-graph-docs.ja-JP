---
title: 組織を更新する
description: organization オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 5037fa0fb14ec327fd24dc3fa12575037487468d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313133"
---
# <a name="update-organization"></a><span data-ttu-id="24562-103">組織を更新する</span><span class="sxs-lookup"><span data-stu-id="24562-103">Update organization</span></span>

> <span data-ttu-id="24562-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24562-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24562-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24562-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24562-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="24562-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24562-107">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="24562-107">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24562-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="24562-108">Prerequisites</span></span>
<span data-ttu-id="24562-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24562-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24562-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="24562-111">Permission type</span></span>|<span data-ttu-id="24562-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="24562-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24562-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="24562-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24562-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24562-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="24562-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="24562-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24562-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24562-116">Not supported.</span></span>|
|<span data-ttu-id="24562-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="24562-117">Application</span></span>|<span data-ttu-id="24562-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24562-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24562-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="24562-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="24562-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24562-120">Request headers</span></span>
|<span data-ttu-id="24562-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="24562-121">Header</span></span>|<span data-ttu-id="24562-122">値</span><span class="sxs-lookup"><span data-stu-id="24562-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24562-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24562-123">Authorization</span></span>|<span data-ttu-id="24562-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="24562-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24562-125">Accept</span><span class="sxs-lookup"><span data-stu-id="24562-125">Accept</span></span>|<span data-ttu-id="24562-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24562-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24562-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="24562-127">Request body</span></span>
<span data-ttu-id="24562-128">要求本文で、[organization](../resources/intune-onboarding-organization.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="24562-128">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="24562-129">次の表に、[organization](../resources/intune-onboarding-organization.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="24562-129">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="24562-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24562-130">Property</span></span>|<span data-ttu-id="24562-131">種類</span><span class="sxs-lookup"><span data-stu-id="24562-131">Type</span></span>|<span data-ttu-id="24562-132">説明</span><span class="sxs-lookup"><span data-stu-id="24562-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24562-133">ID</span><span class="sxs-lookup"><span data-stu-id="24562-133">id</span></span>|<span data-ttu-id="24562-134">String</span><span class="sxs-lookup"><span data-stu-id="24562-134">String</span></span>|<span data-ttu-id="24562-135">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="24562-135">The GUID for the object.</span></span>|
|<span data-ttu-id="24562-136">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="24562-136">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="24562-137">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="24562-137">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="24562-138">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="24562-138">Mobile device management authority.</span></span> <span data-ttu-id="24562-139">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="24562-139">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="24562-140">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="24562-140">certificateConnectorSetting</span></span>|[<span data-ttu-id="24562-141">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="24562-141">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="24562-142">コネクタ証明書の設定です。</span><span class="sxs-lookup"><span data-stu-id="24562-142">Certificate connector setting.</span></span>|



## <a name="response"></a><span data-ttu-id="24562-143">応答</span><span class="sxs-lookup"><span data-stu-id="24562-143">Response</span></span>
<span data-ttu-id="24562-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/intune-onboarding-organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="24562-144">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24562-145">例</span><span class="sxs-lookup"><span data-stu-id="24562-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="24562-146">要求</span><span class="sxs-lookup"><span data-stu-id="24562-146">Request</span></span>
<span data-ttu-id="24562-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="24562-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="24562-148">応答</span><span class="sxs-lookup"><span data-stu-id="24562-148">Response</span></span>
<span data-ttu-id="24562-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="24562-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





