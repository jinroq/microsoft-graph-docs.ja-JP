---
title: GroupPolicyPresentationMultiTextBox の更新
description: GroupPolicyPresentationMultiTextBox オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0dc97d101291b8aa4d83ec522ef7a3d37fd785d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964571"
---
# <a name="update-grouppolicypresentationmultitextbox"></a><span data-ttu-id="6802a-103">GroupPolicyPresentationMultiTextBox の更新</span><span class="sxs-lookup"><span data-stu-id="6802a-103">Update groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="6802a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6802a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6802a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6802a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6802a-106">[Grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6802a-106">Update the properties of a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6802a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6802a-107">Prerequisites</span></span>
<span data-ttu-id="6802a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6802a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6802a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6802a-110">Permission type</span></span>|<span data-ttu-id="6802a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6802a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6802a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6802a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6802a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6802a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6802a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6802a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6802a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6802a-115">Not supported.</span></span>|
|<span data-ttu-id="6802a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6802a-116">Application</span></span>|<span data-ttu-id="6802a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6802a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6802a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6802a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a><span data-ttu-id="6802a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6802a-119">Request headers</span></span>
|<span data-ttu-id="6802a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6802a-120">Header</span></span>|<span data-ttu-id="6802a-121">値</span><span class="sxs-lookup"><span data-stu-id="6802a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6802a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6802a-122">Authorization</span></span>|<span data-ttu-id="6802a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6802a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6802a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6802a-124">Accept</span></span>|<span data-ttu-id="6802a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6802a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6802a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6802a-126">Request body</span></span>
<span data-ttu-id="6802a-127">要求本文で、 [Grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6802a-127">In the request body, supply a JSON representation for the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

<span data-ttu-id="6802a-128">次の表に、 [Grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6802a-128">The following table shows the properties that are required when you create the [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).</span></span>

|<span data-ttu-id="6802a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6802a-129">Property</span></span>|<span data-ttu-id="6802a-130">型</span><span class="sxs-lookup"><span data-stu-id="6802a-130">Type</span></span>|<span data-ttu-id="6802a-131">説明</span><span class="sxs-lookup"><span data-stu-id="6802a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6802a-132">label</span><span class="sxs-lookup"><span data-stu-id="6802a-132">label</span></span>|<span data-ttu-id="6802a-133">String</span><span class="sxs-lookup"><span data-stu-id="6802a-133">String</span></span>|<span data-ttu-id="6802a-134">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="6802a-134">Localized text label for any presentation entity.</span></span> <span data-ttu-id="6802a-135">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="6802a-135">The default value is empty.</span></span> <span data-ttu-id="6802a-136">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6802a-136">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6802a-137">id</span><span class="sxs-lookup"><span data-stu-id="6802a-137">id</span></span>|<span data-ttu-id="6802a-138">String</span><span class="sxs-lookup"><span data-stu-id="6802a-138">String</span></span>|<span data-ttu-id="6802a-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6802a-139">Key of the entity.</span></span> <span data-ttu-id="6802a-140">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6802a-140">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6802a-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6802a-141">lastModifiedDateTime</span></span>|<span data-ttu-id="6802a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6802a-142">DateTimeOffset</span></span>|<span data-ttu-id="6802a-143">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="6802a-143">The date and time the entity was last modified.</span></span> <span data-ttu-id="6802a-144">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6802a-144">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="6802a-145">必須</span><span class="sxs-lookup"><span data-stu-id="6802a-145">required</span></span>|<span data-ttu-id="6802a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="6802a-146">Boolean</span></span>|<span data-ttu-id="6802a-147">テキストボックスに値を入力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6802a-147">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="6802a-148">既定値は False です。</span><span class="sxs-lookup"><span data-stu-id="6802a-148">Default value is false.</span></span>|
|<span data-ttu-id="6802a-149">maxLength</span><span class="sxs-lookup"><span data-stu-id="6802a-149">maxLength</span></span>|<span data-ttu-id="6802a-150">Int64</span><span class="sxs-lookup"><span data-stu-id="6802a-150">Int64</span></span>|<span data-ttu-id="6802a-151">テキストの最大文字数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="6802a-151">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="6802a-152">既定値は1023です。</span><span class="sxs-lookup"><span data-stu-id="6802a-152">Default value is 1023.</span></span>|
|<span data-ttu-id="6802a-153">maxStrings</span><span class="sxs-lookup"><span data-stu-id="6802a-153">maxStrings</span></span>|<span data-ttu-id="6802a-154">Int64</span><span class="sxs-lookup"><span data-stu-id="6802a-154">Int64</span></span>|<span data-ttu-id="6802a-155">文字列の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="6802a-155">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="6802a-156">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="6802a-156">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="6802a-157">応答</span><span class="sxs-lookup"><span data-stu-id="6802a-157">Response</span></span>
<span data-ttu-id="6802a-158">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Grouppolicypresentationmultitextbox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6802a-158">If successful, this method returns a `200 OK` response code and an updated [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6802a-159">例</span><span class="sxs-lookup"><span data-stu-id="6802a-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6802a-160">要求</span><span class="sxs-lookup"><span data-stu-id="6802a-160">Request</span></span>
<span data-ttu-id="6802a-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6802a-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="6802a-162">応答</span><span class="sxs-lookup"><span data-stu-id="6802a-162">Response</span></span>
<span data-ttu-id="6802a-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6802a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```





