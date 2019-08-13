---
title: GroupPolicyPresentationTextBox の更新
description: GroupPolicyPresentationTextBox オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56330e21b7b3243b77dc3d7ad7c15ffec883b927
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357643"
---
# <a name="update-grouppolicypresentationtextbox"></a><span data-ttu-id="6a4c2-103">GroupPolicyPresentationTextBox の更新</span><span class="sxs-lookup"><span data-stu-id="6a4c2-103">Update groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="6a4c2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a4c2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a4c2-106">[Grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-106">Update the properties of a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a4c2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a4c2-107">Prerequisites</span></span>
<span data-ttu-id="6a4c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a4c2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a4c2-110">Permission type</span></span>|<span data-ttu-id="6a4c2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a4c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a4c2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a4c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a4c2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a4c2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a4c2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a4c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a4c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-115">Not supported.</span></span>|
|<span data-ttu-id="6a4c2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a4c2-116">Application</span></span>|<span data-ttu-id="6a4c2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a4c2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a4c2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a4c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="6a4c2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a4c2-119">Request headers</span></span>
|<span data-ttu-id="6a4c2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a4c2-120">Header</span></span>|<span data-ttu-id="6a4c2-121">値</span><span class="sxs-lookup"><span data-stu-id="6a4c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a4c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a4c2-122">Authorization</span></span>|<span data-ttu-id="6a4c2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a4c2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a4c2-124">Accept</span></span>|<span data-ttu-id="6a4c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a4c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a4c2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a4c2-126">Request body</span></span>
<span data-ttu-id="6a4c2-127">要求本文で、 [Grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-127">In the request body, supply a JSON representation for the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

<span data-ttu-id="6a4c2-128">次の表に、 [Grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-128">The following table shows the properties that are required when you create the [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md).</span></span>

|<span data-ttu-id="6a4c2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a4c2-129">Property</span></span>|<span data-ttu-id="6a4c2-130">型</span><span class="sxs-lookup"><span data-stu-id="6a4c2-130">Type</span></span>|<span data-ttu-id="6a4c2-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a4c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a4c2-132">label</span><span class="sxs-lookup"><span data-stu-id="6a4c2-132">label</span></span>|<span data-ttu-id="6a4c2-133">String</span><span class="sxs-lookup"><span data-stu-id="6a4c2-133">String</span></span>|<span data-ttu-id="6a4c2-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6a4c2-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-135">The default value is empty.</span></span> <span data-ttu-id="6a4c2-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6a4c2-137">id</span><span class="sxs-lookup"><span data-stu-id="6a4c2-137">id</span></span>|<span data-ttu-id="6a4c2-138">String</span><span class="sxs-lookup"><span data-stu-id="6a4c2-138">String</span></span>|<span data-ttu-id="6a4c2-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-139">Key of the entity.</span></span> <span data-ttu-id="6a4c2-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6a4c2-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a4c2-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6a4c2-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a4c2-142">DateTimeOffset</span></span>|<span data-ttu-id="6a4c2-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="6a4c2-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6a4c2-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="6a4c2-145">defaultValue</span></span>|<span data-ttu-id="6a4c2-146">String</span><span class="sxs-lookup"><span data-stu-id="6a4c2-146">String</span></span>|<span data-ttu-id="6a4c2-147">テキストボックスに表示されるローカライズされた既定の文字列。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="6a4c2-148">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-148">The default value is empty.</span></span>|
|<span data-ttu-id="6a4c2-149">必須</span><span class="sxs-lookup"><span data-stu-id="6a4c2-149">required</span></span>|<span data-ttu-id="6a4c2-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a4c2-150">Boolean</span></span>|<span data-ttu-id="6a4c2-151">テキストボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="6a4c2-152">既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-152">Default value is false.</span></span>|
|<span data-ttu-id="6a4c2-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="6a4c2-153">maxLength</span></span>|<span data-ttu-id="6a4c2-154">Int64</span><span class="sxs-lookup"><span data-stu-id="6a4c2-154">Int64</span></span>|<span data-ttu-id="6a4c2-155">テキストの最大文字数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="6a4c2-156">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="6a4c2-157">応答</span><span class="sxs-lookup"><span data-stu-id="6a4c2-157">Response</span></span>
<span data-ttu-id="6a4c2-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a4c2-159">例</span><span class="sxs-lookup"><span data-stu-id="6a4c2-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a4c2-160">要求</span><span class="sxs-lookup"><span data-stu-id="6a4c2-160">Request</span></span>
<span data-ttu-id="6a4c2-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a><span data-ttu-id="6a4c2-162">応答</span><span class="sxs-lookup"><span data-stu-id="6a4c2-162">Response</span></span>
<span data-ttu-id="6a4c2-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a4c2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "Label value",
  "id": "ec80633e-633e-ec80-3e63-80ec3e6380ec",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "required": true,
  "maxLength": 9
}
```






