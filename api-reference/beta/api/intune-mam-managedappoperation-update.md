---
title: managedAppOperation の更新
description: managedAppOperation オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6eec0b5068b96330a81ea4d1d305cd7cc5f9e6fe
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985201"
---
# <a name="update-managedappoperation"></a><span data-ttu-id="da2f2-103">managedAppOperation の更新</span><span class="sxs-lookup"><span data-stu-id="da2f2-103">Update managedAppOperation</span></span>

> <span data-ttu-id="da2f2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da2f2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da2f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da2f2-106">[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="da2f2-106">Update the properties of a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da2f2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="da2f2-107">Prerequisites</span></span>
<span data-ttu-id="da2f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da2f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2f2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da2f2-110">Permission type</span></span>|<span data-ttu-id="da2f2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da2f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da2f2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da2f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da2f2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2f2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da2f2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da2f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da2f2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2f2-115">Not supported.</span></span>|
|<span data-ttu-id="da2f2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da2f2-116">Application</span></span>|<span data-ttu-id="da2f2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da2f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da2f2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da2f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="da2f2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da2f2-119">Request headers</span></span>
|<span data-ttu-id="da2f2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da2f2-120">Header</span></span>|<span data-ttu-id="da2f2-121">値</span><span class="sxs-lookup"><span data-stu-id="da2f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da2f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2f2-122">Authorization</span></span>|<span data-ttu-id="da2f2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="da2f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da2f2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="da2f2-124">Accept</span></span>|<span data-ttu-id="da2f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="da2f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2f2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="da2f2-126">Request body</span></span>
<span data-ttu-id="da2f2-127">要求本文で、[managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da2f2-127">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

<span data-ttu-id="da2f2-128">次の表に、[managedAppOperation](../resources/intune-mam-managedappoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="da2f2-128">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune-mam-managedappoperation.md).</span></span>

|<span data-ttu-id="da2f2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da2f2-129">Property</span></span>|<span data-ttu-id="da2f2-130">型</span><span class="sxs-lookup"><span data-stu-id="da2f2-130">Type</span></span>|<span data-ttu-id="da2f2-131">説明</span><span class="sxs-lookup"><span data-stu-id="da2f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2f2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="da2f2-132">displayName</span></span>|<span data-ttu-id="da2f2-133">String</span><span class="sxs-lookup"><span data-stu-id="da2f2-133">String</span></span>|<span data-ttu-id="da2f2-134">操作名。</span><span class="sxs-lookup"><span data-stu-id="da2f2-134">The operation name.</span></span>|
|<span data-ttu-id="da2f2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da2f2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="da2f2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da2f2-136">DateTimeOffset</span></span>|<span data-ttu-id="da2f2-137">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="da2f2-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="da2f2-138">state</span><span class="sxs-lookup"><span data-stu-id="da2f2-138">state</span></span>|<span data-ttu-id="da2f2-139">String</span><span class="sxs-lookup"><span data-stu-id="da2f2-139">String</span></span>|<span data-ttu-id="da2f2-140">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="da2f2-140">The current state of the operation</span></span>|
|<span data-ttu-id="da2f2-141">id</span><span class="sxs-lookup"><span data-stu-id="da2f2-141">id</span></span>|<span data-ttu-id="da2f2-142">String</span><span class="sxs-lookup"><span data-stu-id="da2f2-142">String</span></span>|<span data-ttu-id="da2f2-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="da2f2-143">Key of the entity.</span></span>|
|<span data-ttu-id="da2f2-144">version</span><span class="sxs-lookup"><span data-stu-id="da2f2-144">version</span></span>|<span data-ttu-id="da2f2-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="da2f2-145">String</span></span>|<span data-ttu-id="da2f2-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="da2f2-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="da2f2-147">応答</span><span class="sxs-lookup"><span data-stu-id="da2f2-147">Response</span></span>
<span data-ttu-id="da2f2-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="da2f2-148">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2f2-149">例</span><span class="sxs-lookup"><span data-stu-id="da2f2-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="da2f2-150">要求</span><span class="sxs-lookup"><span data-stu-id="da2f2-150">Request</span></span>
<span data-ttu-id="da2f2-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da2f2-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="da2f2-152">応答</span><span class="sxs-lookup"><span data-stu-id="da2f2-152">Response</span></span>
<span data-ttu-id="da2f2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da2f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




