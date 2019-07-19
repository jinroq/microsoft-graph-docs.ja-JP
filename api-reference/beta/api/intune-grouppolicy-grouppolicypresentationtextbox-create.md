---
title: GroupPolicyPresentationTextBox の作成
description: 新しい groupPolicyPresentationTextBox オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e144f73010f259279b9f71dbd690ae067f8c5521
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964417"
---
# <a name="create-grouppolicypresentationtextbox"></a><span data-ttu-id="27baa-103">GroupPolicyPresentationTextBox の作成</span><span class="sxs-lookup"><span data-stu-id="27baa-103">Create groupPolicyPresentationTextBox</span></span>

> <span data-ttu-id="27baa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27baa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27baa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27baa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27baa-106">新しい[Grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="27baa-106">Create a new [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27baa-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="27baa-107">Prerequisites</span></span>
<span data-ttu-id="27baa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27baa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27baa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27baa-110">Permission type</span></span>|<span data-ttu-id="27baa-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27baa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27baa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27baa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27baa-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27baa-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="27baa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27baa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27baa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27baa-115">Not supported.</span></span>|
|<span data-ttu-id="27baa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27baa-116">Application</span></span>|<span data-ttu-id="27baa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27baa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27baa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27baa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="27baa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27baa-119">Request headers</span></span>
|<span data-ttu-id="27baa-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27baa-120">Header</span></span>|<span data-ttu-id="27baa-121">値</span><span class="sxs-lookup"><span data-stu-id="27baa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27baa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27baa-122">Authorization</span></span>|<span data-ttu-id="27baa-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="27baa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27baa-124">承諾</span><span class="sxs-lookup"><span data-stu-id="27baa-124">Accept</span></span>|<span data-ttu-id="27baa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27baa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27baa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="27baa-126">Request body</span></span>
<span data-ttu-id="27baa-127">要求本文で、groupPolicyPresentationTextBox オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27baa-127">In the request body, supply a JSON representation for the groupPolicyPresentationTextBox object.</span></span>

<span data-ttu-id="27baa-128">次の表に、groupPolicyPresentationTextBox の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27baa-128">The following table shows the properties that are required when you create the groupPolicyPresentationTextBox.</span></span>

|<span data-ttu-id="27baa-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27baa-129">Property</span></span>|<span data-ttu-id="27baa-130">型</span><span class="sxs-lookup"><span data-stu-id="27baa-130">Type</span></span>|<span data-ttu-id="27baa-131">説明</span><span class="sxs-lookup"><span data-stu-id="27baa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27baa-132">label</span><span class="sxs-lookup"><span data-stu-id="27baa-132">label</span></span>|<span data-ttu-id="27baa-133">String</span><span class="sxs-lookup"><span data-stu-id="27baa-133">String</span></span>|<span data-ttu-id="27baa-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="27baa-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="27baa-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="27baa-135">The default value is empty.</span></span> <span data-ttu-id="27baa-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="27baa-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="27baa-137">id</span><span class="sxs-lookup"><span data-stu-id="27baa-137">id</span></span>|<span data-ttu-id="27baa-138">String</span><span class="sxs-lookup"><span data-stu-id="27baa-138">String</span></span>|<span data-ttu-id="27baa-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="27baa-139">Key of the entity.</span></span> <span data-ttu-id="27baa-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="27baa-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="27baa-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27baa-141">lastModifiedDateTime</span></span>|<span data-ttu-id="27baa-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27baa-142">DateTimeOffset</span></span>|<span data-ttu-id="27baa-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="27baa-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="27baa-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="27baa-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="27baa-145">defaultValue</span><span class="sxs-lookup"><span data-stu-id="27baa-145">defaultValue</span></span>|<span data-ttu-id="27baa-146">String</span><span class="sxs-lookup"><span data-stu-id="27baa-146">String</span></span>|<span data-ttu-id="27baa-147">テキストボックスに表示されるローカライズされた既定の文字列。</span><span class="sxs-lookup"><span data-stu-id="27baa-147">Localized default string displayed in the text box.</span></span> <span data-ttu-id="27baa-148">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="27baa-148">The default value is empty.</span></span>|
|<span data-ttu-id="27baa-149">必須</span><span class="sxs-lookup"><span data-stu-id="27baa-149">required</span></span>|<span data-ttu-id="27baa-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="27baa-150">Boolean</span></span>|<span data-ttu-id="27baa-151">テキストボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="27baa-151">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="27baa-152">既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="27baa-152">Default value is false.</span></span>|
|<span data-ttu-id="27baa-153">maxLength</span><span class="sxs-lookup"><span data-stu-id="27baa-153">maxLength</span></span>|<span data-ttu-id="27baa-154">Int64</span><span class="sxs-lookup"><span data-stu-id="27baa-154">Int64</span></span>|<span data-ttu-id="27baa-155">テキストの最大文字数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="27baa-155">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="27baa-156">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="27baa-156">Default value is 1023.</span></span>|



## <a name="response"></a><span data-ttu-id="27baa-157">応答</span><span class="sxs-lookup"><span data-stu-id="27baa-157">Response</span></span>
<span data-ttu-id="27baa-158">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27baa-158">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27baa-159">例</span><span class="sxs-lookup"><span data-stu-id="27baa-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="27baa-160">要求</span><span class="sxs-lookup"><span data-stu-id="27baa-160">Request</span></span>
<span data-ttu-id="27baa-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27baa-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
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

### <a name="response"></a><span data-ttu-id="27baa-162">応答</span><span class="sxs-lookup"><span data-stu-id="27baa-162">Response</span></span>
<span data-ttu-id="27baa-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27baa-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





