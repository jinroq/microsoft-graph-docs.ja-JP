---
title: GroupPolicyPresentationText の更新
description: GroupPolicyPresentationText オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dc02044db74e92f51b0cfdd706af3135a5c9a557
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35989365"
---
# <a name="update-grouppolicypresentationtext"></a><span data-ttu-id="afb9c-103">GroupPolicyPresentationText の更新</span><span class="sxs-lookup"><span data-stu-id="afb9c-103">Update groupPolicyPresentationText</span></span>

> <span data-ttu-id="afb9c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afb9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afb9c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="afb9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afb9c-106">[Grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-106">Update the properties of a [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afb9c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="afb9c-107">Prerequisites</span></span>
<span data-ttu-id="afb9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afb9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb9c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afb9c-110">Permission type</span></span>|<span data-ttu-id="afb9c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="afb9c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afb9c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afb9c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afb9c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb9c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="afb9c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afb9c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afb9c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afb9c-115">Not supported.</span></span>|
|<span data-ttu-id="afb9c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afb9c-116">Application</span></span>|<span data-ttu-id="afb9c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afb9c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afb9c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afb9c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="afb9c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afb9c-119">Request headers</span></span>
|<span data-ttu-id="afb9c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afb9c-120">Header</span></span>|<span data-ttu-id="afb9c-121">値</span><span class="sxs-lookup"><span data-stu-id="afb9c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afb9c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="afb9c-122">Authorization</span></span>|<span data-ttu-id="afb9c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="afb9c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afb9c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="afb9c-124">Accept</span></span>|<span data-ttu-id="afb9c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afb9c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afb9c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="afb9c-126">Request body</span></span>
<span data-ttu-id="afb9c-127">要求本文で、 [Grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-127">In the request body, supply a JSON representation for the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object.</span></span>

<span data-ttu-id="afb9c-128">次の表に、 [Grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-128">The following table shows the properties that are required when you create the [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).</span></span>

|<span data-ttu-id="afb9c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afb9c-129">Property</span></span>|<span data-ttu-id="afb9c-130">型</span><span class="sxs-lookup"><span data-stu-id="afb9c-130">Type</span></span>|<span data-ttu-id="afb9c-131">説明</span><span class="sxs-lookup"><span data-stu-id="afb9c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb9c-132">label</span><span class="sxs-lookup"><span data-stu-id="afb9c-132">label</span></span>|<span data-ttu-id="afb9c-133">String</span><span class="sxs-lookup"><span data-stu-id="afb9c-133">String</span></span>|<span data-ttu-id="afb9c-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="afb9c-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="afb9c-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="afb9c-135">The default value is empty.</span></span> <span data-ttu-id="afb9c-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="afb9c-137">id</span><span class="sxs-lookup"><span data-stu-id="afb9c-137">id</span></span>|<span data-ttu-id="afb9c-138">String</span><span class="sxs-lookup"><span data-stu-id="afb9c-138">String</span></span>|<span data-ttu-id="afb9c-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="afb9c-139">Key of the entity.</span></span> <span data-ttu-id="afb9c-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="afb9c-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afb9c-141">lastModifiedDateTime</span></span>|<span data-ttu-id="afb9c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb9c-142">DateTimeOffset</span></span>|<span data-ttu-id="afb9c-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="afb9c-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="afb9c-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|



## <a name="response"></a><span data-ttu-id="afb9c-145">応答</span><span class="sxs-lookup"><span data-stu-id="afb9c-145">Response</span></span>
<span data-ttu-id="afb9c-146">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Grouppolicypresentationtext](../resources/intune-grouppolicy-grouppolicypresentationtext.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="afb9c-146">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb9c-147">例</span><span class="sxs-lookup"><span data-stu-id="afb9c-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="afb9c-148">要求</span><span class="sxs-lookup"><span data-stu-id="afb9c-148">Request</span></span>
<span data-ttu-id="afb9c-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afb9c-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 96

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value"
}
```

### <a name="response"></a><span data-ttu-id="afb9c-150">応答</span><span class="sxs-lookup"><span data-stu-id="afb9c-150">Response</span></span>
<span data-ttu-id="afb9c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afb9c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "Label value",
  "id": "bc77d545-d545-bc77-45d5-77bc45d577bc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





