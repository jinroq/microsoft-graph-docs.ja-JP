---
title: termsAndConditionsAcceptanceStatus の更新
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 726257a07a268bb2475e84d545a8c63b21c40431
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790747"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="1e422-103">termsAndConditionsAcceptanceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="1e422-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="1e422-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e422-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e422-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e422-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e422-106">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1e422-106">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e422-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e422-107">Prerequisites</span></span>
<span data-ttu-id="1e422-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e422-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e422-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e422-110">Permission type</span></span>|<span data-ttu-id="1e422-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e422-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e422-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e422-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e422-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e422-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1e422-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e422-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e422-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e422-115">Not supported.</span></span>|
|<span data-ttu-id="1e422-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e422-116">Application</span></span>|<span data-ttu-id="1e422-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e422-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e422-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e422-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="1e422-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e422-119">Request headers</span></span>
|<span data-ttu-id="1e422-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e422-120">Header</span></span>|<span data-ttu-id="1e422-121">値</span><span class="sxs-lookup"><span data-stu-id="1e422-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e422-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e422-122">Authorization</span></span>|<span data-ttu-id="1e422-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e422-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e422-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1e422-124">Accept</span></span>|<span data-ttu-id="1e422-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e422-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e422-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e422-126">Request body</span></span>
<span data-ttu-id="1e422-127">要求本文で、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e422-127">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="1e422-128">次の表に、[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1e422-128">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="1e422-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e422-129">Property</span></span>|<span data-ttu-id="1e422-130">型</span><span class="sxs-lookup"><span data-stu-id="1e422-130">Type</span></span>|<span data-ttu-id="1e422-131">説明</span><span class="sxs-lookup"><span data-stu-id="1e422-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e422-132">id</span><span class="sxs-lookup"><span data-stu-id="1e422-132">id</span></span>|<span data-ttu-id="1e422-133">String</span><span class="sxs-lookup"><span data-stu-id="1e422-133">String</span></span>|<span data-ttu-id="1e422-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1e422-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1e422-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1e422-135">userDisplayName</span></span>|<span data-ttu-id="1e422-136">String</span><span class="sxs-lookup"><span data-stu-id="1e422-136">String</span></span>|<span data-ttu-id="1e422-137">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1e422-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="1e422-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="1e422-138">acceptedVersion</span></span>|<span data-ttu-id="1e422-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1e422-139">Int32</span></span>|<span data-ttu-id="1e422-140">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="1e422-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="1e422-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e422-141">acceptedDateTime</span></span>|<span data-ttu-id="1e422-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e422-142">DateTimeOffset</span></span>|<span data-ttu-id="1e422-143">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1e422-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="1e422-144">応答</span><span class="sxs-lookup"><span data-stu-id="1e422-144">Response</span></span>
<span data-ttu-id="1e422-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e422-145">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e422-146">例</span><span class="sxs-lookup"><span data-stu-id="1e422-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e422-147">要求</span><span class="sxs-lookup"><span data-stu-id="1e422-147">Request</span></span>
<span data-ttu-id="1e422-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e422-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="1e422-149">応答</span><span class="sxs-lookup"><span data-stu-id="1e422-149">Response</span></span>
<span data-ttu-id="1e422-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e422-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





