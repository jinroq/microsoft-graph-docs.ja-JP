---
title: managedAppOperation の更新
description: managedAppOperation オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 2bd0d326a4300bdae29484b547bbd5aa429728ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311978"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="b5f55-103">managedAppOperation の更新</span><span class="sxs-lookup"><span data-stu-id="b5f55-103">Update managedAppOperation</span></span>

> <span data-ttu-id="b5f55-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b5f55-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5f55-105">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b5f55-105">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b5f55-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b5f55-106">Prerequisites</span></span>
<span data-ttu-id="b5f55-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5f55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5f55-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5f55-109">Permission type</span></span>|<span data-ttu-id="b5f55-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5f55-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5f55-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5f55-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b5f55-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5f55-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5f55-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5f55-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5f55-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5f55-114">Not supported.</span></span>|
|<span data-ttu-id="b5f55-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5f55-115">Application</span></span>|<span data-ttu-id="b5f55-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5f55-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5f55-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5f55-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5f55-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5f55-118">Request headers</span></span>
|<span data-ttu-id="b5f55-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5f55-119">Header</span></span>|<span data-ttu-id="b5f55-120">値</span><span class="sxs-lookup"><span data-stu-id="b5f55-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5f55-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5f55-121">Authorization</span></span>|<span data-ttu-id="b5f55-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b5f55-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5f55-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b5f55-123">Accept</span></span>|<span data-ttu-id="b5f55-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b5f55-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5f55-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5f55-125">Request body</span></span>
<span data-ttu-id="b5f55-126">要求本文で、[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b5f55-126">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="b5f55-127">次の表に、[managedAppOperation](../resources/intune-mam-managedappoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b5f55-127">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="b5f55-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5f55-128">Property</span></span>|<span data-ttu-id="b5f55-129">種類</span><span class="sxs-lookup"><span data-stu-id="b5f55-129">Type</span></span>|<span data-ttu-id="b5f55-130">説明</span><span class="sxs-lookup"><span data-stu-id="b5f55-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5f55-131">displayName</span><span class="sxs-lookup"><span data-stu-id="b5f55-131">displayName</span></span>|<span data-ttu-id="b5f55-132">String</span><span class="sxs-lookup"><span data-stu-id="b5f55-132">String</span></span>|<span data-ttu-id="b5f55-133">操作名。</span><span class="sxs-lookup"><span data-stu-id="b5f55-133">The operation name.</span></span>|
|<span data-ttu-id="b5f55-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5f55-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b5f55-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5f55-135">DateTimeOffset</span></span>|<span data-ttu-id="b5f55-136">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="b5f55-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="b5f55-137">state</span><span class="sxs-lookup"><span data-stu-id="b5f55-137">state</span></span>|<span data-ttu-id="b5f55-138">String</span><span class="sxs-lookup"><span data-stu-id="b5f55-138">String</span></span>|<span data-ttu-id="b5f55-139">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="b5f55-139">The current state of the operation</span></span>|
|<span data-ttu-id="b5f55-140">id</span><span class="sxs-lookup"><span data-stu-id="b5f55-140">id</span></span>|<span data-ttu-id="b5f55-141">String</span><span class="sxs-lookup"><span data-stu-id="b5f55-141">String</span></span>|<span data-ttu-id="b5f55-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b5f55-142">Key of the entity.</span></span>|
|<span data-ttu-id="b5f55-143">version</span><span class="sxs-lookup"><span data-stu-id="b5f55-143">version</span></span>|<span data-ttu-id="b5f55-144">String</span><span class="sxs-lookup"><span data-stu-id="b5f55-144">String</span></span>|<span data-ttu-id="b5f55-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b5f55-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b5f55-146">応答</span><span class="sxs-lookup"><span data-stu-id="b5f55-146">Response</span></span>
<span data-ttu-id="b5f55-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b5f55-147">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5f55-148">例</span><span class="sxs-lookup"><span data-stu-id="b5f55-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="b5f55-149">要求</span><span class="sxs-lookup"><span data-stu-id="b5f55-149">Request</span></span>
<span data-ttu-id="b5f55-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b5f55-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="b5f55-151">応答</span><span class="sxs-lookup"><span data-stu-id="b5f55-151">Response</span></span>
<span data-ttu-id="b5f55-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b5f55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```



