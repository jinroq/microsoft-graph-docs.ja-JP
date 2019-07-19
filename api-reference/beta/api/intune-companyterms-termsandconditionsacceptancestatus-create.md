---
title: termsAndConditionsAcceptanceStatus の作成
description: 新しい termsAndConditionsAcceptanceStatus オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8b5a9a16e907b2d375efe97ff99d665c5838a0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34971970"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="6a88b-103">termsAndConditionsAcceptanceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="6a88b-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="6a88b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a88b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a88b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a88b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a88b-106">新しい [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a88b-106">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a88b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a88b-107">Prerequisites</span></span>
<span data-ttu-id="6a88b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a88b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a88b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a88b-110">Permission type</span></span>|<span data-ttu-id="6a88b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a88b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a88b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a88b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a88b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a88b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a88b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a88b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a88b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a88b-115">Not supported.</span></span>|
|<span data-ttu-id="6a88b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a88b-116">Application</span></span>|<span data-ttu-id="6a88b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a88b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a88b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a88b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6a88b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a88b-119">Request headers</span></span>
|<span data-ttu-id="6a88b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a88b-120">Header</span></span>|<span data-ttu-id="6a88b-121">値</span><span class="sxs-lookup"><span data-stu-id="6a88b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a88b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a88b-122">Authorization</span></span>|<span data-ttu-id="6a88b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a88b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a88b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a88b-124">Accept</span></span>|<span data-ttu-id="6a88b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a88b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a88b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a88b-126">Request body</span></span>
<span data-ttu-id="6a88b-127">要求本文で、termsAndConditionsAcceptanceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a88b-127">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="6a88b-128">次の表に、termsAndConditionsAcceptanceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a88b-128">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="6a88b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a88b-129">Property</span></span>|<span data-ttu-id="6a88b-130">型</span><span class="sxs-lookup"><span data-stu-id="6a88b-130">Type</span></span>|<span data-ttu-id="6a88b-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a88b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a88b-132">id</span><span class="sxs-lookup"><span data-stu-id="6a88b-132">id</span></span>|<span data-ttu-id="6a88b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6a88b-133">String</span></span>|<span data-ttu-id="6a88b-134">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6a88b-134">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="6a88b-135">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a88b-135">userDisplayName</span></span>|<span data-ttu-id="6a88b-136">String</span><span class="sxs-lookup"><span data-stu-id="6a88b-136">String</span></span>|<span data-ttu-id="6a88b-137">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="6a88b-137">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="6a88b-138">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="6a88b-138">acceptedVersion</span></span>|<span data-ttu-id="6a88b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6a88b-139">Int32</span></span>|<span data-ttu-id="6a88b-140">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="6a88b-140">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="6a88b-141">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a88b-141">acceptedDateTime</span></span>|<span data-ttu-id="6a88b-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a88b-142">DateTimeOffset</span></span>|<span data-ttu-id="6a88b-143">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6a88b-143">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="6a88b-144">応答</span><span class="sxs-lookup"><span data-stu-id="6a88b-144">Response</span></span>
<span data-ttu-id="6a88b-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a88b-145">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a88b-146">例</span><span class="sxs-lookup"><span data-stu-id="6a88b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a88b-147">要求</span><span class="sxs-lookup"><span data-stu-id="6a88b-147">Request</span></span>
<span data-ttu-id="6a88b-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a88b-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="6a88b-149">応答</span><span class="sxs-lookup"><span data-stu-id="6a88b-149">Response</span></span>
<span data-ttu-id="6a88b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a88b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





