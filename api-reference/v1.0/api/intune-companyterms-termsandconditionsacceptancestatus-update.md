---
title: termsAndConditionsAcceptanceStatus の更新
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 06169225518f6110cb571d53ba818cd8fece49e7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019766"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="7d74a-103">termsAndConditionsAcceptanceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="7d74a-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="7d74a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d74a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d74a-105">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7d74a-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d74a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7d74a-106">Prerequisites</span></span>
<span data-ttu-id="7d74a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d74a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d74a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d74a-109">Permission type</span></span>|<span data-ttu-id="7d74a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d74a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d74a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d74a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d74a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d74a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7d74a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d74a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d74a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d74a-114">Not supported.</span></span>|
|<span data-ttu-id="7d74a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d74a-115">Application</span></span>|<span data-ttu-id="7d74a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d74a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d74a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d74a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="7d74a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d74a-118">Request headers</span></span>
|<span data-ttu-id="7d74a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d74a-119">Header</span></span>|<span data-ttu-id="7d74a-120">値</span><span class="sxs-lookup"><span data-stu-id="7d74a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d74a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d74a-121">Authorization</span></span>|<span data-ttu-id="7d74a-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7d74a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d74a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="7d74a-123">Accept</span></span>|<span data-ttu-id="7d74a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d74a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d74a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d74a-125">Request body</span></span>
<span data-ttu-id="7d74a-126">要求本文で、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7d74a-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="7d74a-127">次の表に、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7d74a-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="7d74a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d74a-128">Property</span></span>|<span data-ttu-id="7d74a-129">型</span><span class="sxs-lookup"><span data-stu-id="7d74a-129">Type</span></span>|<span data-ttu-id="7d74a-130">説明</span><span class="sxs-lookup"><span data-stu-id="7d74a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d74a-131">id</span><span class="sxs-lookup"><span data-stu-id="7d74a-131">id</span></span>|<span data-ttu-id="7d74a-132">文字列</span><span class="sxs-lookup"><span data-stu-id="7d74a-132">String</span></span>|<span data-ttu-id="7d74a-133">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7d74a-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7d74a-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7d74a-134">userDisplayName</span></span>|<span data-ttu-id="7d74a-135">String</span><span class="sxs-lookup"><span data-stu-id="7d74a-135">String</span></span>|<span data-ttu-id="7d74a-136">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="7d74a-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="7d74a-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="7d74a-137">acceptedVersion</span></span>|<span data-ttu-id="7d74a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7d74a-138">Int32</span></span>|<span data-ttu-id="7d74a-139">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="7d74a-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="7d74a-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d74a-140">acceptedDateTime</span></span>|<span data-ttu-id="7d74a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d74a-141">DateTimeOffset</span></span>|<span data-ttu-id="7d74a-142">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7d74a-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="7d74a-143">応答</span><span class="sxs-lookup"><span data-stu-id="7d74a-143">Response</span></span>
<span data-ttu-id="7d74a-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7d74a-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d74a-145">例</span><span class="sxs-lookup"><span data-stu-id="7d74a-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d74a-146">要求</span><span class="sxs-lookup"><span data-stu-id="7d74a-146">Request</span></span>
<span data-ttu-id="7d74a-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7d74a-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="7d74a-148">応答</span><span class="sxs-lookup"><span data-stu-id="7d74a-148">Response</span></span>
<span data-ttu-id="7d74a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7d74a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



