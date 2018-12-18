---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
ms.openlocfilehash: d32eb2b06cb76c578edf4a80e73e5bf6ec6b4757
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334455"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

すべて学校データ プロファイルの id の同期設定の抽象基本クラスです。 派生クラスは、識別情報を同期するための動作を定義します。 派生型を次に示します。

## <a name="derived-types"></a>派生型
| 種類 | 説明 | 
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | Azure Active Directory (AD の Azure) 内の既存のユーザー アカウントを一致させるには、この型を使用します。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | Azure AD で新しいユーザー アカウントを作成するのにには、この型を使用します。 |
