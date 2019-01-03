---
title: managedAppOperation の更新
description: managedAppOperation オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 3ec9e327f1eae83eca31661742c241cec58740bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312944"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="63892-103">managedAppOperation の更新</span><span class="sxs-lookup"><span data-stu-id="63892-103">Update managedAppOperation</span></span>

> <span data-ttu-id="63892-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63892-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63892-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63892-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63892-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="63892-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63892-107">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="63892-107">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="63892-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="63892-108">Prerequisites</span></span>
<span data-ttu-id="63892-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63892-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63892-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63892-111">Permission type</span></span>|<span data-ttu-id="63892-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="63892-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63892-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63892-113">Delegated (work or school account)</span></span>|<span data-ttu-id="63892-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63892-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="63892-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63892-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63892-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63892-116">Not supported.</span></span>|
|<span data-ttu-id="63892-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63892-117">Application</span></span>|<span data-ttu-id="63892-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63892-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63892-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63892-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="63892-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63892-120">Request headers</span></span>
|<span data-ttu-id="63892-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63892-121">Header</span></span>|<span data-ttu-id="63892-122">値</span><span class="sxs-lookup"><span data-stu-id="63892-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63892-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63892-123">Authorization</span></span>|<span data-ttu-id="63892-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="63892-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63892-125">Accept</span><span class="sxs-lookup"><span data-stu-id="63892-125">Accept</span></span>|<span data-ttu-id="63892-126">application/json</span><span class="sxs-lookup"><span data-stu-id="63892-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63892-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="63892-127">Request body</span></span>
<span data-ttu-id="63892-128">要求本文で、[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="63892-128">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="63892-129">次の表に、[managedAppOperation](../resources/intune-mam-managedappoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="63892-129">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="63892-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63892-130">Property</span></span>|<span data-ttu-id="63892-131">種類</span><span class="sxs-lookup"><span data-stu-id="63892-131">Type</span></span>|<span data-ttu-id="63892-132">説明</span><span class="sxs-lookup"><span data-stu-id="63892-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63892-133">displayName</span><span class="sxs-lookup"><span data-stu-id="63892-133">displayName</span></span>|<span data-ttu-id="63892-134">String</span><span class="sxs-lookup"><span data-stu-id="63892-134">String</span></span>|<span data-ttu-id="63892-135">操作名。</span><span class="sxs-lookup"><span data-stu-id="63892-135">The operation name.</span></span>|
|<span data-ttu-id="63892-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="63892-136">lastModifiedDateTime</span></span>|<span data-ttu-id="63892-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63892-137">DateTimeOffset</span></span>|<span data-ttu-id="63892-138">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="63892-138">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="63892-139">state</span><span class="sxs-lookup"><span data-stu-id="63892-139">state</span></span>|<span data-ttu-id="63892-140">String</span><span class="sxs-lookup"><span data-stu-id="63892-140">String</span></span>|<span data-ttu-id="63892-141">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="63892-141">The current state of the operation</span></span>|
|<span data-ttu-id="63892-142">id</span><span class="sxs-lookup"><span data-stu-id="63892-142">id</span></span>|<span data-ttu-id="63892-143">String</span><span class="sxs-lookup"><span data-stu-id="63892-143">String</span></span>|<span data-ttu-id="63892-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="63892-144">Key of the entity.</span></span>|
|<span data-ttu-id="63892-145">version</span><span class="sxs-lookup"><span data-stu-id="63892-145">version</span></span>|<span data-ttu-id="63892-146">String</span><span class="sxs-lookup"><span data-stu-id="63892-146">String</span></span>|<span data-ttu-id="63892-147">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="63892-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="63892-148">応答</span><span class="sxs-lookup"><span data-stu-id="63892-148">Response</span></span>
<span data-ttu-id="63892-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="63892-149">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63892-150">例</span><span class="sxs-lookup"><span data-stu-id="63892-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="63892-151">要求</span><span class="sxs-lookup"><span data-stu-id="63892-151">Request</span></span>
<span data-ttu-id="63892-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="63892-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 165

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="63892-153">応答</span><span class="sxs-lookup"><span data-stu-id="63892-153">Response</span></span>
<span data-ttu-id="63892-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="63892-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




