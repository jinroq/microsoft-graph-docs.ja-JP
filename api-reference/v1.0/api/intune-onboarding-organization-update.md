---
title: 組織を更新する
description: organization オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: d26d11bb2f67b933ba5d78e444ae8e52d32339ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358899"
---
# <a name="update-organization"></a><span data-ttu-id="e0b97-103">organization の更新</span><span class="sxs-lookup"><span data-stu-id="e0b97-103">Update organization</span></span>

> <span data-ttu-id="e0b97-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0b97-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0b97-105">[organization](../resources/intune-onboarding-organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0b97-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0b97-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0b97-106">Prerequisites</span></span>
<span data-ttu-id="e0b97-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0b97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0b97-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0b97-109">Permission type</span></span>|<span data-ttu-id="e0b97-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0b97-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0b97-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0b97-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0b97-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0b97-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e0b97-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0b97-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0b97-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0b97-114">Not supported.</span></span>|
|<span data-ttu-id="e0b97-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0b97-115">Application</span></span>|<span data-ttu-id="e0b97-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0b97-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0b97-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0b97-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0b97-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0b97-118">Request headers</span></span>
|<span data-ttu-id="e0b97-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0b97-119">Header</span></span>|<span data-ttu-id="e0b97-120">値</span><span class="sxs-lookup"><span data-stu-id="e0b97-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0b97-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0b97-121">Authorization</span></span>|<span data-ttu-id="e0b97-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e0b97-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0b97-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e0b97-123">Accept</span></span>|<span data-ttu-id="e0b97-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e0b97-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0b97-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0b97-125">Request body</span></span>
<span data-ttu-id="e0b97-126">要求本文で、[organization](../resources/intune-onboarding-organization.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0b97-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="e0b97-127">次の表に、[organization](../resources/intune-onboarding-organization.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e0b97-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="e0b97-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0b97-128">Property</span></span>|<span data-ttu-id="e0b97-129">種類</span><span class="sxs-lookup"><span data-stu-id="e0b97-129">Type</span></span>|<span data-ttu-id="e0b97-130">説明</span><span class="sxs-lookup"><span data-stu-id="e0b97-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0b97-131">ID</span><span class="sxs-lookup"><span data-stu-id="e0b97-131">id</span></span>|<span data-ttu-id="e0b97-132">String</span><span class="sxs-lookup"><span data-stu-id="e0b97-132">String</span></span>|<span data-ttu-id="e0b97-133">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="e0b97-133">The GUID for the object.</span></span>|
|<span data-ttu-id="e0b97-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="e0b97-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="e0b97-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="e0b97-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="e0b97-136">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="e0b97-136">Mobile device management authority.</span></span> <span data-ttu-id="e0b97-137">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="e0b97-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="e0b97-138">応答</span><span class="sxs-lookup"><span data-stu-id="e0b97-138">Response</span></span>
<span data-ttu-id="e0b97-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/intune-onboarding-organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e0b97-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0b97-140">例</span><span class="sxs-lookup"><span data-stu-id="e0b97-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0b97-141">要求</span><span class="sxs-lookup"><span data-stu-id="e0b97-141">Request</span></span>
<span data-ttu-id="e0b97-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0b97-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="e0b97-143">応答</span><span class="sxs-lookup"><span data-stu-id="e0b97-143">Response</span></span>
<span data-ttu-id="e0b97-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0b97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



